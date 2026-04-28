# OpenClaw Coding Skills

**别再指望 Agent “刚好能行”。把可靠的 coding 行为变成默认。**

面向 OpenClaw Agent 的生产级 coding skills 仓库。

它也是 MyClaw.ai 生态的一部分，目标不是单纯堆 prompt，而是把 Agent 驱动的软件开发进一步工程化、结构化、可持续调优。

这个项目做的不是“让模型更聪明”，而是“让 Agent 在真实 coding 任务里更像成熟工程师”。它通过一套 workflow skills、specialist skills、执行支架、触发映射、评估样本和调优闭环，把原本容易漂移的 coding 行为，收束成更稳定、更可验证、更可复用的执行系统。

## 这个项目提供什么

- 工作流 skills：`spec`、`plan`、`build`、`test`、`review`、`ship`
- 专项 skills：`debug`、`security`、`frontend`、`docs`、`deploy`、`refactor`
- `references/` 执行支架：帮助 agent 在关键决策点减少拍脑袋和误判
- `TRIGGER-MATRIX`：提升自动触发命中率和边界清晰度
- `examples/`：真实请求样本，用来校准触发质量
- `evaluation/`：带标签评估集、歧义样本、dry-run validation、live validation、调优闭环

换句话说，它不是单个 prompt，也不是几个 skill 的堆叠，而是一套围绕真实 coding 工作流构建的行为优化系统。

## 核心价值

它提升的不是模型权重，而是 coding 行为质量。

很多 Agent 在软件开发里翻车，不是因为不会写代码，而是因为执行方式不够成熟：范围没定义清楚就开写、改动面太大、验证证据太弱、review 和 test 混在一起、高风险任务没有足够支架。

这个项目的价值，就是系统性降低这些失败模式：

- 更会先定义范围，再动代码
- 更会分小步推进，而不是一把梭
- 更会在宣布完成前要求足够证据
- 更会处理 debug、安全、部署、重构这些高风险场景
- 更容易通过样本、评估和 live validation 持续调优

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
