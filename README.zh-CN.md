[English](README.md) | [简体中文](README.zh-CN.md)

# Novel Writing Kit

一个面向中文小说创作的 Codex plugin，同时兼容 Claude 的本地 skill 目录格式。

## 核心 Skills

- `novel-architect`：建立故事圣经、人物、世界规则、时间线和创作约束。
- `novel-outline`：规划主线、分卷、章节、场景、冲突和钩子。
- `novel-draft`：续写、补写、扩写、改写和重写正文。
- `novel-continuity`：检查人物、时间线、规则、资源、信息差和伏笔。
- `novel-prose-edit`：审校中文表达、对白、节奏、重复和 AI 腔。
- `novel-research`：按需核验历史、地理和专业事实。
- `novel-memory`：维护状态卡、进度、伏笔池、章节摘要和上下文压缩。

`novel-orchestrator` 是用于多步骤任务的可选路由器。

## 使用方式

- 简单任务直接调用对应的核心 skill。
- 多步骤任务调用 `novel-orchestrator`。
- 需要确定性路由时，可以显式调用 `$novel-draft` 等 skill。

完整路由协议见 [`plugins/novel-writing-kit/docs/routing.md`](plugins/novel-writing-kit/docs/routing.md)。

## 范围与隐私

本项目不包含人物样例、私人聊天、真实人物档案或固定小说设定。使用者应在自己的小说项目中添加这些内容。

## 许可证与来源

本项目采用 MIT License，见 [`LICENSE`](LICENSE)。来源整理、隐私排除和改编记录见 [`PROVENANCE.md`](PROVENANCE.md)。贡献规范见 [`CONTRIBUTING.md`](CONTRIBUTING.md)。
