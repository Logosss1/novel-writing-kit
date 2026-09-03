# Skill Routing

本文件是 Novel Writing Kit 的统一路由表。它描述“什么时候用哪个 skill”，不替代各 skill 的详细规则。

## 入口原则

| 场景 | 入口 |
| --- | --- |
| 简单、单一交付物 | 直接调用一个核心 skill |
| 多步骤小说任务 | 调用可选的 `novel-orchestrator` |
| 用户明确指定 skill | 优先执行用户指定的 skill |

## 任务路由

| 任务类型 | 主 skill | 后续 skill |
| --- | --- | --- |
| 新建小说项目 | `novel-architect` | `novel-outline` |
| 设定重构 | `novel-architect` | `novel-continuity` |
| 故事、分卷、章节大纲 | `novel-outline` | `novel-memory`（有状态变化时） |
| 续写、补写、扩写、重写 | `novel-draft` | `novel-prose-edit` -> `novel-continuity` -> `novel-memory` |
| 正文涉及真实知识 | `novel-research` | `novel-draft` 或 `novel-continuity` |
| 语言润色 | `novel-prose-edit` | 通常结束 |
| 设定与剧情检查 | `novel-continuity` | 回到产生问题的 skill 修复 |
| 上下文整理或压缩 | `novel-memory` | 通常结束 |

## 推荐调用链

### 新项目

```text
novel-architect -> novel-outline
```

### 完整章节工作流

```text
novel-memory -> novel-draft -> novel-research(按需)
-> novel-prose-edit -> novel-continuity -> novel-memory
```

### 单一任务

```text
“润色这段话”       -> novel-prose-edit
“查这个历史细节”   -> novel-research
“检查人物是否 OOC” -> novel-continuity
“压缩旧章节”       -> novel-memory
```

## 交接要求

阶段交接至少说明：完成内容、依据文件、状态变化、阻塞项和下一步。若没有状态变化，不要强制调用 `novel-memory`；若没有现实世界断言，不要调用 `novel-research`。
