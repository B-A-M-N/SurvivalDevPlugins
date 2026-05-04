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
**Mistral Vibe workflow design, implementation, and validation lifecycle**

Single-model Claude Code plugin for conceptualizing, designing, planning, applying, and validating advanced Mistral Vibe workflows. VibeFlow uses signed intent artifacts, progressive feasibility references, Mermaid/JSON runtime diagrams, and deterministic validation gates to keep workflow designs grounded in real Mistral Vibe internals.

- Lifecycle: `init → design → plan → apply → validate`
- Init emits signed `VISION.md`, `PLAN.md`, and `WORKFLOW_CONTRACT.json`
- Design maps intent to feasible runtime surfaces instead of assuming impossible middleware/tool/session behavior
- Feasibility substrate covers tiers A-E, key contracts, workflow patterns, events, config keys, tier composition, and observability

### [Converge](https://github.com/B-A-M-N/converge)
**Universal recurring task engine for CLI AI agents**

Automates recurring tasks, scheduled workflows, and loop-based execution for AI agents running in CLI environments.

- Cron-based scheduling with natural language support
- Loop execution with self-paced cadence
- Background task management and wake-up calls

### [PRForge](https://github.com/B-A-M-N/prforge)
**Professional PR contribution harness for Claude Code**

Delegated PR execution with guarded release, coding discipline enforcement, and distributed mesh mode. Turns the agent into a disciplined upstream contributor.

- Model: investigate → plan → patch → validate → self-review → package → you approve
- Enforces repo intelligence, scope contracts, validation honesty, and git safety
- Distributed mesh mode for multi-repo contribution workflows

## Installation

Add the SurvivalDev marketplace:

```bash
claude plugin marketplace add B-A-M-N/SurvivalDevPlugins
```

List available plugins:

```bash
claude plugin list
```

Install a plugin:

```bash
claude plugin install handshake@survivaldev-plugins
claude plugin install vibeflow@survivaldev-plugins
claude plugin install survivaldev-infradoctor@survivaldev-plugins
claude plugin install converge@survivaldev-plugins
claude plugin install prforge@survivaldev-plugins
```

## Topics

Browse all plugins by topic: [`claude-code`](https://github.com/topics/claude-code) [`plugin`](https://github.com/topics/plugin) [`survivaldev`](https://github.com/topics/survivaldev)
