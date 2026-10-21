# Agency Specialists — ChatGPT/Codex Plugin

A curated, skills-only Plugin conversion of selected workflows from [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents).

## Included workflows

- **Code Review** — prioritized findings across correctness, security, maintainability, performance, and testing.
- **UX Research Planner** — research questions, methodology, participant criteria, ethics, analysis, and evidence-linked recommendations.
- **Content Campaign Planner** — audience, positioning, editorial pillars, channel adaptations, measurement, and experiment design.
- **Multi-role Project Runbook** — decomposes a project into roles, phases, dependencies, acceptance criteria, and decision gates.
- **Host Workspace Operator** — safe, capability-oriented guidance for repository/file work.
- **Python Evidence Executor** — deterministic checks and reportable evidence when Python is available.

## Why skills-only

These workflows encode decision processes, templates, and review standards. They use tools supplied by the host and require no bundled MCP server, credentials, telemetry, or external runtime.

## Installation / use

This is a plugin package root. The manifest is in `.codex-plugin/plugin.json`; Skills are in `skills/`. Check current ChatGPT/Codex plugin installation instructions for your host before enabling it. This repository addition has not been live-smoke-tested in ChatGPT or Codex.

## Source and license

Adapted from the MIT-licensed [The Agency repository](https://github.com/msitarzewski/agency-agents). This is a curated conversion, not a mirror of the full agent roster. See `CONVERSION-REPORT.md` for source dispositions, validation evidence, and limitations.

No Plugin Directory submission or release is implied by this repository change.