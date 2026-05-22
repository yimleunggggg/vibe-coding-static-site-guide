# SEO 自动化文档

面向 **静态站点 + GitHub Actions**。案例：[yakushimabus.com](https://yakushimabus.com)。

> 本仓库**全部公开**；填 Secret 请用 [SETUP_CHECKLIST.md](SETUP_CHECKLIST.md) 复制到本地，勿提交真实值。

## 从哪里开始

| 你是… | 读这个 |
|--------|--------|
| **从零跟做（推荐）** | **[tutorial/README.md](tutorial/README.md)** |
| 填 Secret / 邮箱（本地） | [SETUP_CHECKLIST.md](SETUP_CHECKLIST.md) |
| 总流程 | [RUNBOOK.md](RUNBOOK.md) |
| 通知 | [NOTIFICATIONS.md](NOTIFICATIONS.md) |
| 飞书（可选） | [FEISHU_SETUP.md](FEISHU_SETUP.md) |
| 需求与进度 | [ROADMAP.md](ROADMAP.md) |
| 指标表模板 | [TRACKING.md](TRACKING.md) |

## 定时任务一览

| 任务 | 北京时间 | 产出 |
|------|----------|------|
| 日报 | 每天 17:00 | 报告 + 可选 ntfy/邮件 |
| 半月 | 1/15 日 17:00 | reminder + Issue |
| 周报 | 周一 17:30 | 方案 + Issue |

## Cursor 优化轮

定时任务**默认不改** meta；复杂改版可用 Cursor，或周报 Issue 回复 `approve`。
