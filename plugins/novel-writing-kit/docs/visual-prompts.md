# Workflow Visual Prompts

这份文档提供适合 README、项目主页或发布介绍页的工作流配图方向。提示词强调专业的软件工具感，不包含真实人物、私人资料或具体小说角色。

仓库内已提供对应的轻量 SVG 配图，适合直接嵌入 GitHub README。

## 1. Overall Architecture

![Overall architecture](assets/overall-architecture.svg)

**用途**：展示 Novel Writing Kit 是一套分工明确的中文小说创作系统。

**Image prompt**

> Professional editorial workflow diagram for a Chinese novel writing toolkit, clean white background, deep charcoal typography, restrained red accent, seven clearly labeled modules arranged around a central manuscript: Architect, Outline, Draft, Research, Prose Edit, Continuity, Memory. Thin directional lines show information flowing from story foundation to finished chapter and back into project memory. Minimal vector-infographic style, precise spacing, high legibility, no decorative characters, no gradients, no lorem ipsum, landscape 16:9.

## 2. Chapter Production Loop

![Chapter production loop](assets/chapter-production-loop.svg)

**用途**：展示单章从准备到交付的完整流程。

**Image prompt**

> Elegant product workflow illustration for a Chinese fiction chapter pipeline. A manuscript page moves through six sequential stations: state context, draft scene, research facts when needed, edit prose, check continuity, update memory. Use numbered stages, compact labels, clear arrows, subtle paper and ink motifs, white and cool gray palette with one vermilion accent, editorial software documentation aesthetic, no human figures, no fantasy imagery, landscape 16:9.

## 3. Task Routing Map

![Task routing map](assets/task-routing-map.svg)

**用途**：解释简单任务和多步骤任务如何选择 skill。

**Image prompt**

> High-end systems diagram showing task routing for a novel-writing assistant. On the left, four input cards: initialize a novel, plan an outline, write a chapter, polish a paragraph. A central router classifies each request. On the right, routes connect to the smallest suitable module, while complex chapter requests follow a longer sequence through draft, research, prose edit, continuity, and memory. Crisp grid, black text, white background, muted blue-gray lines, one red highlight for the router, professional developer-tool documentation style, landscape 16:9.

## 4. Memory and Context Compression

![Memory and context compression](assets/memory-compression.svg)

**用途**：展示 `novel-memory` 如何把长篇内容转成可持续使用的项目记忆。

**Image prompt**

> Professional information-management diagram for long-form Chinese novel memory. On the left, a tall stack of chapter pages and notes; in the center, a careful compression process separates durable facts, current state, timeline, resources, and foreshadowing; on the right, a compact project memory index and recent-chapter window remain available for the next session. Visual language of archival folders and structured metadata, clean white background, charcoal and teal with a single amber accent, no characters, no fantasy symbols, high legibility, landscape 16:9.

## 5. Quality Control Triangle

![Quality control triangle](assets/quality-control-triangle.svg)

**用途**：展示正文生成后的三类质量保障。

**Image prompt**

> Minimal editorial quality-control diagram for Chinese novel writing. A finished manuscript sits at the center of a triangle with three labeled pillars: narrative continuity, prose quality, factual credibility. Each pillar contains small visual cues for characters and timeline, sentence rhythm and dialogue, research sources and historical details. Refined publishing-tool aesthetic, generous whitespace, dark graphite typography, muted green and red accents, no people, no decorative gradients, landscape 16:9.

## 使用建议

- README 首页优先使用“Overall Architecture”。
- 介绍章节工作流时使用“Chapter Production Loop”。
- 解释 orchestrator 时使用“Task Routing Map”。
- 介绍 `novel-memory` 时使用“Memory and Context Compression”。
- 图片中文字应使用英文模块名，避免生成模型产生难以辨认的中文小字；中文说明放在图片下方。
