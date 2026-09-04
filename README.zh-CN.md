[English](README.md) | [简体中文](README.zh-CN.md)

# Novel Writing Kit（自用）

一个面向中文小说创作的 Codex plugin，同时兼容 Claude 的本地 skill 目录格式。

## 核心 Skills

- `novel-architect`：建立故事框架、人物系统、世界规则、时间线和创作约束。
- `novel-outline`：把创意拆解为主线、分卷、章节、场景、冲突和章末钩子。
- `novel-draft`：在保持人物动机、叙事视角和场景承接的前提下创作与改写正文。
- `novel-continuity`：审查人物、时间线、规则、资源、信息差、伤势和伏笔。
- `novel-prose-edit`：优化中文表达、对白、节奏、重复、语气和 AI 腔。
- `novel-research`：按需核验历史、地理、制度、医学、军事和科技细节。
- `novel-memory`：跨会话维护状态卡、进度、伏笔池、章节摘要和上下文压缩。

`novel-orchestrator` 是用于多步骤任务的可选路由器。

## 使用方式

- 简单任务直接调用对应的核心 skill。
- 多步骤任务调用 `novel-orchestrator`。
- 需要确定性路由时，可以显式调用 `$novel-draft` 等 skill。

完整路由协议见 [`plugins/novel-writing-kit/docs/routing.md`](plugins/novel-writing-kit/docs/routing.md)。

## 工作流程概览

整个套件遵循一条可控的创作闭环：建立设定、规划剧情、创作章节、按需核验事实、编辑语言、审查连续性，最后更新项目记忆。简单任务可以直接调用单个 skill，多步骤任务可以使用可选的 orchestrator。

![Novel Writing Kit 工作流](plugins/novel-writing-kit/docs/assets/overall-architecture.svg)

工作流图示和图片生成描述见 [`docs/visual-prompts.md`](plugins/novel-writing-kit/docs/visual-prompts.md)。

## 范围与隐私

本项目不包含人物样例、私人聊天、真实人物档案或固定小说设定。使用者应在自己的小说项目中添加这些内容。

## 许可证与来源

本项目采用 MIT License，见 [`LICENSE`](LICENSE)。来源整理、隐私排除和改编记录见 [`PROVENANCE.md`](PROVENANCE.md)。贡献规范见 [`CONTRIBUTING.md`](CONTRIBUTING.md)。
