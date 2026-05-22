# 发布到 GitHub（维护者用）

## 推送

```bash
cd ~/你的教程库目录/vibe-coding-static-site-guide
git remote set-url origin git@github.com:你的GitHub用户名/vibe-coding-static-site-guide.git
git push origin main
```

## 分享链接

- 首页：`https://github.com/你的GitHub用户名/vibe-coding-static-site-guide`
- Playbook：`.../tree/main/playbook`
- SEO 教程：`.../tree/main/seo/tutorial`

## 与主项目代码库同步

案例站点源码在独立仓库（如 `Yakushima-bus`）。更新教程时，从主项目的 `docs/playbook/`、`docs/seo/tutorial/` 等复制到本库，**勿复制**含本地路径、真实邮箱的文件。
