# 配置清单（模板）

> **本仓库全部公开。** 请在你**自己电脑**复制本文件填写（如 `my-setup.local.md`），**勿**把真实密钥、邮箱、Token 提交到 GitHub。

公开步骤见 [tutorial/README.md](tutorial/README.md)。

## 我的站点

| 项 | 我的值 |
|----|--------|
| 域名 | `https://_______________/` |
| GSC 资源 URL | 与上相同 |
| GA4 衡量 ID（埋点） | `G-________` |
| GA4 属性 ID（API，纯数字） | `________` |
| Cloud 项目 ID | `_______________` |
| 服务账号邮箱 | `____________@____________.iam.gserviceaccount.com` |

## Google 本地文件（仅本机 `secrets/`，勿提交）

- [ ] `secrets/google-sa.json`
- [ ] `secrets/oauth-client.json`
- [ ] `secrets/oauth-refresh.txt`

## GitHub Secrets 勾选表

- [ ] `GOOGLE_SERVICE_ACCOUNT_JSON`
- [ ] `GOOGLE_OAUTH_CLIENT_JSON`
- [ ] `GOOGLE_OAUTH_REFRESH_TOKEN`
- [ ] `GA4_PROPERTY_ID`
- [ ] `GSC_SITE_URL`
- [ ] `SEO_NOTIFY_EMAIL`
- [ ] `RESEND_API_KEY`
- [ ] `RESEND_FROM`
- [ ] `NTFY_TOPIC`
- [ ] （可选）`FEISHU_APP_ID` / `FEISHU_APP_SECRET` / `FEISHU_FOLDER_TOKEN`

## 验证记录

| 日期 | 操作 | 结果 |
|------|------|------|
| | Actions SEO daily | |
| | ntfy / 邮件 | |
| | 周报 Issue | |
