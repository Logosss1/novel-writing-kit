# Workflow Visual Prompts

这份文档提供适合 README、项目主页或发布介绍页的工作流配图方向。提示词强调专业的软件工具感，不包含真实人物、私人资料或具体小说角色。

仓库内已提供对应的轻量 SVG 配图，适合直接嵌入 GitHub README。

## 1. Overall Architecture

![Overall architecture](assets/overall-architecture.svg)

**用途**：展示 Novel Writing Kit 是一套分工明确的中文小说创作系统。


## 2. Chapter Production Loop

![Chapter production loop](assets/chapter-production-loop.svg)

**用途**：展示单章从准备到交付的完整流程。

## 3. Task Routing Map

![Task routing map](assets/task-routing-map.svg)

**用途**：解释简单任务和多步骤任务如何选择 skill。


## 4. Memory and Context Compression

![Memory and context compression](assets/memory-compression.svg)

**用途**：展示 `novel-memory` 如何把长篇内容转成可持续使用的项目记忆。


## 5. Quality Control Triangle

![Quality control triangle](assets/quality-control-triangle.svg)

**用途**：展示正文生成后的三类质量保障。


## 使用建议

- README 首页优先使用“Overall Architecture”。
- 介绍章节工作流时使用“Chapter Production Loop”。
- 解释 orchestrator 时使用“Task Routing Map”。
- 介绍 `novel-memory` 时使用“Memory and Context Compression”。
- 图片中文字应使用英文模块名，避免生成模型产生难以辨认的中文小字；中文说明放在图片下方。
