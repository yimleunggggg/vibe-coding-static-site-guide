# Vibe Coding 工具站教程 · 案例 Yakushima Bus

> 用 Cursor 对话做产品，约 **2 个密集工作日** 从零上线 [yakushimabus.com](https://yakushimabus.com)，并接好 **GA4/GSC 自动日报**（每天 17:00 推手机 + 邮件）。  
> 本文库 **脱敏、可分享**；完整代码与脚本见主仓库 [Yakushima-bus](https://github.com/yimleunggggg/Yakushima-bus)。

---

## 从这里开始

| 你想… | 打开 |
|--------|------|
| **总故事 + 架构 + 踩坑**（发社媒首选） | [playbook/README.md](playbook/README.md) |
| **跟做 SEO 自动化**（Actions / 通知） | [seo/tutorial/README.md](seo/tutorial/README.md) |
| **部署 GitHub Pages + 域名** | [deploy/github-pages-custom-domain.md](deploy/github-pages-custom-domain.md) |
| **案例产品是什么** | [case-study/product-intro.md](case-study/product-intro.md) |
| **脚本与 workflow 源码** | [CODE_REFERENCE.md](CODE_REFERENCE.md) |

---

## 教程结构

```text
playbook/          01～08：vibe coding 流程、架构、复用清单
seo/
  tutorial/        01～05 + 排错：Google 授权、Actions、通知
  README.md        SEO 文档索引
  RUNBOOK.md       从零到跑通总流程
  NOTIFICATIONS.md 邮件 + ntfy
  FEISHU_SETUP.md  飞书（可选）
  ROADMAP.md       需求与进度
deploy/            域名 + DNS + Pages
case-study/        屋久岛公交工具站产品介绍
```

---

## 本库涵盖什么

1. **怎么做一个小而美的静态工具站**（官方 PDF → 脚本 → 网页）  
2. **怎么绑域名、免费托管**  
3. **怎么让 Google 数据每天自动流到你手机**（不必 Cursor、不必电脑开机）  
4. **真实踩坑**：GSC 服务账号加不进去、OAuth、Resend DNS、新站 0 展示等  
5. **下一个项目怎么复用**（清单 + 可拷贝的 workflow 说明）

术语均有人话解释，面向 **不会写代码、但会用 AI 做产品** 的读者。

---

## 案例链接

- 线上站点：https://yakushimabus.com  
- 源代码：https://github.com/yimleunggggg/Yakushima-bus  

---

## 私人配置

自己填 Secret 用 [seo/PRIVATE_SETUP.md](seo/PRIVATE_SETUP.md)（模板，勿提交真实密钥）。
