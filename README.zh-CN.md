# OpenClaw Coding Skills

面向 OpenClaw Agent 的生产级 coding skills 仓库。

它也是 MyClaw.ai 生态的一部分，定位不是单纯堆 prompt，而是把 Agent 驱动的软件开发进一步产品化、工程化、可调优化。

这个项目不是去改变底层模型本身，而是通过一套工程化 skills、触发映射、评估样本和调优闭环，让 OpenClaw 在真实开发任务中表现得更稳、更严谨、更像成熟工程师。

## 这个项目提供什么

- 工作流 skills：`spec`、`plan`、`build`、`test`、`review`、`ship`
- 专项 skills：`debug`、`security`、`frontend`、`docs`、`deploy`、`refactor`
- `references/` 执行支架：帮助 agent 在关键决策点更少拍脑袋
- `TRIGGER-MATRIX`：提升自动触发命中率
- `examples/`：真实请求样本
- `evaluation/`：带标签评估集、歧义样本、调优闭环

## 核心价值

它提升的不是模型权重，而是工程行为质量：

- 更会先定义范围，再动代码
- 更会拆步骤，而不是一把梭
- 更会要求证据，而不是自信宣布完成
- 更会处理 debug、安全、部署、重构这些高风险场景
- 更容易通过样本和评估持续调优触发效果

## 适合谁

- 希望 OpenClaw 在 coding 任务里更稳定的团队
- 希望把工程规范沉淀成可复用 skills 的团队
- 希望持续调优 agent 行为，而不是只调 prompt 的团队

## 入口

- 英文主文档：[README.md](./README.md)
- 安装说明：[INSTALL.md](./INSTALL.md)
- 采用指南：[ADOPTION-GUIDE.md](./ADOPTION-GUIDE.md)
- 触发映射：[skills/TRIGGER-MATRIX.md](./skills/TRIGGER-MATRIX.md)
- 示例任务集：[examples/README.md](./examples/README.md)
- 评估与调优：[evaluation/README.md](./evaluation/README.md)
