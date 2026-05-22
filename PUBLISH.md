# 发布到 GitHub（一次性）

本地仓库已就绪：`/Users/yimleung/手搓程序/Yakushima-bus-guides`（已 commit）。

## 步骤

1. 打开 https://github.com/new  
2. Repository name：`Yakushima-bus-guides`  
3. Public，**不要**勾选 Add README  
4. Create repository  
5. 终端执行：

```bash
cd "/Users/yimleung/手搓程序/Yakushima-bus-guides"
git remote set-url origin https://github.com/yimleunggggg/Yakushima-bus-guides.git
git push -u origin main
```

## 分享链接

- 首页：https://github.com/yimleunggggg/Yakushima-bus-guides  
- Playbook：https://github.com/yimleunggggg/Yakushima-bus-guides/tree/main/playbook  
- SEO 教程：https://github.com/yimleunggggg/Yakushima-bus-guides/tree/main/seo/tutorial  

## 与主项目同步

主代码仓库：[Yakushima-bus](https://github.com/yimleunggggg/Yakushima-bus)  
更新教程后，从 `docs/playbook/`、`docs/seo/tutorial/` 等复制到本库并 push。
