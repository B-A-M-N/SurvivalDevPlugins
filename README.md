# SurvivalDev Plugins

A collection of context-continuity and workflow-survival plugins for Claude Code.

## Plugins

### [Handshake](https://github.com/B-A-M-N/handshake)
**Context-continuity for Claude Code**

Prevents agent memory loss during compaction, `/clear`, or long-running sessions. Automatically checkpoints workflow state before context reset and rehydrates after.

- Hook-driven: `PreCompact`, `SessionStart`, `UserPromptSubmit`
- Skill-driven toggle: `/handshake on|off|status`
- Checkpoint format: structured JSON (machine) + Markdown (human)

### [SurvivalDev-InfraDoctor](https://github.com/B-A-M-N/survivaldev-infradoctor)
**Infrastructure doctor for self-hosted services**

Hook-driven diagnostics and repair for self-hosted Firecrawl and SearXNG instances. Detects failures, diagnoses root causes, applies safe repairs, and validates recovery.

- Autonomous diagnosis → propose fix → safe repair → validate → report loop
- Dispatched automatically on infrastructure incidents

### [VibeFlow](https://github.com/B-A-M-N/vibeflow)
**Visual workflow orchestration for Claude Code**

*Repository coming soon.*

### [Converge](https://github.com/B-A-M-N/converge)
**Universal recurring task engine for CLI AI agents**

Automates recurring tasks, scheduled workflows, and loop-based execution for AI agents running in CLI environments.

- Cron-based scheduling with natural language support
- Loop execution with self-paced cadence
- Background task management and wake-up calls

## Usage

Each plugin lives in its own repo. Install by cloning or loading via `--plugin-dir`:

```bash
claude --plugin-dir /path/to/handshake
```

## Topics

Browse all plugins by topic: [`claude-code`](https://github.com/topics/claude-code) [`plugin`](https://github.com/topics/plugin) [`survivaldev`](https://github.com/topics/survivaldev)
