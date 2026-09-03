# Novel Writing Kit

面向中文小说创作的 Codex plugin，也可作为 Claude 的本地 skill 目录使用。

## 核心 Skills

- `novel-architect`：建立小说设定、人物、规则与创作约束。
- `novel-outline`：规划主线、分卷、章节和场景推进。
- `novel-draft`：续写、改写、扩写和重写正文。
- `novel-continuity`：检查人物、时间线、规则、资源和伏笔一致性。
- `novel-prose-edit`：检查中文表达、节奏、对话和 AI 腔。
- `novel-research`：按需核验历史、地理和专业事实。
- `novel-memory`：维护状态卡、伏笔池、章节摘要和上下文压缩。

## 可选 Skill

- `novel-orchestrator`：协调多个 skill 的调用顺序和报告频率。

## 如何选择

- 简单任务直接调用对应的核心 skill，例如润色用 `novel-prose-edit`，查资料用 `novel-research`。
- 多步骤任务调用可选的 `novel-orchestrator`，由它先识别任务，再按路由表串联必要 skill。
- 用户也可以显式指定 `$novel-architect`、`$novel-draft` 等 skill；显式指定优先于自动扩展。

完整路由表见 [`docs/routing.md`](docs/routing.md)。

## 使用方式

在 Codex 中安装此 plugin 后，可直接描述小说任务；也可以显式调用对应 skill。Claude 用户可将 `skills/` 下的 skill 目录复制到自己的 skills 目录。

本项目不提供人物样例和具体小说设定。使用者应在自己的项目中添加人物卡、世界观、章节和状态文件。
