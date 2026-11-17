# Orion Computer Use

An open-source project exploring verifiable computer use for AI agents.

Orion Computer Use aims to help an AI worker operate desktop applications and report **what actually happened**, with evidence that a manager or human can inspect. Its first milestone is a small, local macOS workflow—not a general-purpose autonomous desktop agent.

> **Status: planning.** This repository currently contains project goals and an MVP plan only. No desktop control, agent, MCP server, or benchmark has been implemented yet.

## Why

Agents can plan tasks, but a click or a successful tool call does not prove a task was completed. We want to explore how a worker can perform a bounded desktop task, check its actual result, and return a clear success or failure report. Over time, this may support the Manager/Worker workflows developed in the [Orion Agents](https://github.com/orion-agents) ecosystem.

## v0.1.0: the first milestone

The planned MVP targets a single local worker on macOS. It will perform one repeatable, non-sensitive task using TextEdit and a project-owned workspace, verify the resulting file, and produce a structured report. See the [v0.1.0 plan](docs/plan/v0.1.0.md) for the precise task, boundaries, and acceptance criteria.

The MVP is planned to use a deterministic task definition. It does **not** require a model API, a trained model, or an NVIDIA GPU. The desktop-control implementation and dependencies are still to be evaluated; no existing driver has been selected or integrated.

## Documentation

- [Project goals](docs/goal.md) — motivation, users, principles, and long-term direction.
- [v0.1.0 MVP plan](docs/plan/v0.1.0.md) — scope, implementation sequence, and measurable acceptance criteria.

## 中文简介

Orion Computer Use 是一个探索 **AI Worker 可靠操作电脑并提供可验证结果** 的开源项目。首个版本计划在 macOS 上完成一个本地、可重复的桌面任务，检查最终文件，并输出清晰的成功或失败报告。当前项目处于规划阶段，尚无可运行实现。

## Contributing

Issues and pull requests are welcome. During the planning phase, useful contributions include concrete use cases, corrections, and comparisons with existing desktop automation tools. Please discuss substantial design changes in an issue before implementing them. Do not include secrets, private screenshots, or personal files in examples or reports.

## License

[MIT](LICENSE)
