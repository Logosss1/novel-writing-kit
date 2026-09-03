# Novel Writing Kit

面向中文小说创作的 Codex plugin，也可作为 Claude 的本地 skill 目录使用。

## 核心 Skills

- `novel-architect`：建立故事圣经、人物系统、世界规则、时间线和创作约束。
- `novel-outline`：把创意拆解为主线、分卷、章节、场景、冲突和章末钩子。
- `novel-draft`：在保持人物动机、叙事视角和场景承接的前提下创作与改写正文。
- `novel-continuity`：审查人物、时间线、规则、资源、信息差、伤势和伏笔。
- `novel-prose-edit`：优化中文表达、对白、节奏、重复、语气和 AI 腔。
- `novel-research`：按需核验历史、地理、制度、医学、军事和科技细节。
- `novel-memory`：跨会话维护状态卡、进度、伏笔池、章节摘要和上下文压缩。

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
