# 部署：GitHub Pages + 自定义域名

> **本教程案例**：yakushimabus.com（屋久岛公交查询）。下面用 `你的域名.com`、`你的GitHub用户名` 作占位，照换即可。  
> 纯静态站，无构建步骤；推送 `main` 分支根目录即可。

---

## 阶段 A：域名审核期间（可先上线）

域名在注册商实名审核时，**先用 GitHub 默认地址**，不耽误开发。

1. **推送代码**
   ```bash
   cd ~/你的项目目录
   git push origin main
   ```

2. **开启 Pages**  
   仓库 `你的GitHub用户名/你的仓库名` → **Settings → Pages**  
   - Source：`Deploy from a branch`  
   - Branch：`main` / **/** (root)  
   - Custom domain：**先留空**（填了自定义域名但 DNS 未就绪会报错，正常）

3. **预览地址**（约 1～2 分钟）  
   `https://你的GitHub用户名.github.io/你的仓库名/`

---

## 阶段 B：域名生效后

### 1. DNS 解析（以腾讯云 DNSPod 为例）

根域名添加 **4 条 A 记录**（GitHub Pages **公共 IP**，所有人相同）：

| 记录类型 | 主机记录 | 记录值 | TTL |
|----------|----------|--------|-----|
| A | @ | 185.199.108.153 | 600 |
| A | @ | 185.199.109.153 | 600 |
| A | @ | 185.199.110.153 | 600 |
| A | @ | 185.199.111.153 | 600 |

可选 www：

| CNAME | www | 你的GitHub用户名.github.io | 600 |

> 案例：`yakushimabus.com` 即按上表配置；**Resend 邮件**另需 `send` / `resend._domainkey` 等记录，与网站 A 记录不冲突。

### 2. GitHub 绑定域名

Settings → Pages → Custom domain 填 **`你的域名.com`** → Save → 等 DNS 生效 → **Enforce HTTPS**。

仓库根目录 `CNAME` 文件内容一行：`你的域名.com`。

### 3. 验证

```bash
dig 你的域名.com +short
curl -I https://你的域名.com
```

---

## 首次推送（新仓库）

```bash
cd ~/你的项目目录
git init
git add .
git commit -m "Initial deploy"
git branch -M main
git remote add origin https://github.com/你的GitHub用户名/你的仓库名.git
git push -u origin main
```

---

## 日后更新

```bash
git add -A && git commit -m "update" && git push
```

Pages 约 1～2 分钟自动更新。

---

## 常见问题

| 问题 | 处理 |
|------|------|
| 404 | Pages 源为 `main` 根目录；确认有 `index.html` |
| InvalidDNSError | DNS 未生效或 A 记录未配齐；审核期先用 github.io |
| HTTPS 灰掉 | 等 DNS 全生效后再开 Enforce HTTPS |

---

## 备选托管

- **Cloudflare Pages** / **Vercel**：连同一 GitHub 仓库，Build 留空，Output `/`
