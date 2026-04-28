# SurvivalDev Plugins

A collection of context-continuity and workflow-survival plugins for Claude Code.

## Plugins

### [Handshake](https://github.com/B-A-M-N/handshake)
**Context-continuity for Claude Code**

Prevents agent memory loss during compaction, `/clear`, or long-running sessions. Automatically checkpoints workflow state before context reset and rehydrates after.

- Hook-driven: `PreCompact`, `SessionStart`, `UserPromptSubmit`
- Skill-driven toggle: `/handshake on|off|status`
- Checkpoint format: structured JSON (machine) + Markdown (human)

## Usage

Each plugin lives in its own repo. Install by cloning or loading via `--plugin-dir`:

```bash
claude --plugin-dir /path/to/handshake
```

## Topics

Browse all plugins by topic: [`claude-code`](https://github.com/topics/claude-code) [`plugin`](https://github.com/topics/plugin) [`survivaldev`](https://github.com/topics/survivaldev)
