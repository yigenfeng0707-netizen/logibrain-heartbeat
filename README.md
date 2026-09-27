# LogiBrain Heartbeat

线上服务心跳监控：每 10 分钟检查一次 https://yunliyuan.cn（后端 /api/v1/health + 前端 /onto 页面）。

- 检查失败 → 自动创建 🔴 告警 issue（@yigenfeng0707-netizen，含处理预案）
- 恢复正常 → 自动关闭未决告警并留恢复记录
- 每月 1 日自动提交一次 keepalive commit，防止 GitHub 因 60 天无仓库活动而停用定时任务

> 背景：2026-09 发现生产后端自 09-01 起停机近 4 周无人知晓。本仓库即为此教训的对策。
