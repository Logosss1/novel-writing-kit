[English](README.md) | [简体中文](README.zh-CN.md)

# Novel Writing Kit

A Codex plugin for structured Chinese novel writing, also usable as a local skill collection in Claude.

## Core skills

- `novel-architect`: story bible, characters, world rules, timeline, and constraints.
- `novel-outline`: arcs, volumes, chapters, scenes, conflict, and hooks.
- `novel-draft`: drafting, continuation, expansion, rewriting, and chapter handoff.
- `novel-continuity`: characters, timeline, rules, resources, information gaps, and foreshadowing.
- `novel-prose-edit`: Chinese prose, dialogue, rhythm, repetition, and AI-like phrasing.
- `novel-research`: on-demand fact checking for historical, geographic, and professional details.
- `novel-memory`: state cards, progress, hook ledgers, summaries, and context compression.

`novel-orchestrator` is an optional router for multi-step tasks.

## Usage

- Use a single core skill for a focused task.
- Use `novel-orchestrator` for multi-step workflows.
- Explicitly invoke a skill such as `$novel-draft` when deterministic routing is preferred.

See [`plugins/novel-writing-kit/docs/routing.md`](plugins/novel-writing-kit/docs/routing.md) for the routing contract.

## Scope and privacy

This repository contains no character samples, private chats, real-person profiles, or fixed novel setting. Add those only in your own novel project.

## License and provenance

Released under the MIT License; see [`LICENSE`](LICENSE). Source reorganization, privacy exclusions, and adaptation notes are documented in [`PROVENANCE.md`](PROVENANCE.md). Contributions are covered by [`CONTRIBUTING.md`](CONTRIBUTING.md).
