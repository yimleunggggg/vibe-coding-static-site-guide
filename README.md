# Vibe Coding 静态工具站从 0 到 1 使用教程

> **案例**：屋久岛公交查询 [yakushimabus.com](https://yakushimabus.com)  
> 用 Cursor 对话做产品，约 **2 个密集工作日** 上线站点，并接好 **GA4/GSC 自动日报**（每天 17:00 推手机 + 邮件）。  
> 本库 **脱敏、可分享**；完整代码见 [Yakushima-bus](https://github.com/yimleunggggg/Yakushima-bus)。

---

## 适合谁读

不会写代码、但会用 **AI（Vibe Coding）** 做**小而美工具站**的人——例如：时刻表、换算器、本地生活查询、旅行交通工具等。

---

## 从这里开始

| 你想… | 打开 |
|--------|------|
| **总流程 + 架构 + 踩坑**（发社媒首选） | [playbook/README.md](playbook/README.md) |
| **跟做 SEO 自动化**（Actions / 通知） | [seo/tutorial/README.md](seo/tutorial/README.md) |
| **部署 GitHub Pages + 域名** | [deploy/github-pages-custom-domain.md](deploy/github-pages-custom-domain.md) |
| **本案例产品功能说明** | [case-study/product-intro.md](case-study/product-intro.md) |
| **脚本源码在哪** | [CODE_REFERENCE.md](CODE_REFERENCE.md) |

---

## 教程结构

```text
playbook/          01～08：从想法到上线、架构、复用清单
seo/
  tutorial/        01～05 + 排错：Google 授权、Actions、通知
  README.md        SEO 文档索引
deploy/            域名 + DNS + Pages
case-study/        屋久岛公交案例（产品介绍）
```

---

## 本教程涵盖什么

1. 怎么做**静态工具站**（官方 PDF → 脚本 → 网页）  
2. 怎么**绑域名、免费托管**  
3. 怎么让 **Google 数据每天自动推到手机**（不必 Cursor、不必电脑开机）  
4. **真实踩坑**：GSC 授权、OAuth、Resend DNS、新站 0 展示等  
5. **下一个类似项目怎么复用**

术语均有人话解释。

---

## 私人配置

自己填 Secret：[seo/PRIVATE_SETUP.md](seo/PRIVATE_SETUP.md)（模板，勿提交真实密钥）。
