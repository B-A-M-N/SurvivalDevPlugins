# SurvivalDev Plugins

A Claude Code plugin marketplace. Context-continuity and workflow-survival plugins.

## Installation

Add the SurvivalDev marketplace:

```bash
claude plugin marketplace add B-A-M-N/SurvivalDevPlugins
```

Install any plugin:

```bash
claude plugin install handshake@survivaldev-plugins
claude plugin install vibeflow@survivaldev-plugins
claude plugin install survivaldev-infradoctor@survivaldev-plugins
claude plugin install converge@survivaldev-plugins
claude plugin install prforge@survivaldev-plugins
```

Check installed plugins:

```bash
claude plugin list
```

## Plugins

| Plugin | Source | Description |
|---|---|---|
| **handshake** | [`B-A-M-N/handshake`](https://github.com/B-A-M-N/handshake) | Context-continuity — checkpoints workflow state before compaction/clear and rehydrates after |
| **survivaldev-infradoctor** | [`B-A-M-N/survivaldev-infradoctor`](https://github.com/B-A-M-N/survivaldev-infradoctor) | Infrastructure doctor for self-hosted Firecrawl and SearXNG |
| **vibeflow** | [`B-A-M-N/vibeflow`](https://github.com/B-A-M-N/vibeflow) | Mistral Vibe workflow design, implementation, and validation lifecycle |
| **converge** | [`B-A-M-N/converge`](https://github.com/B-A-M-N/converge) | Universal recurring task engine — cron, loops, background tasks |
| **prforge** | [`B-A-M-N/prforge`](https://github.com/B-A-M-N/prforge) | Professional PR contribution harness with guarded release and mesh mode |

### handshake

Prevents agent memory loss during compaction, `/clear`, or long-running sessions. Automatically checkpoints workflow state before context reset and rehydrates after.

- Hook-driven: `PreCompact`, `SessionStart`, `UserPromptSubmit`
- Skill-driven toggle: `/handshake on|off|status`
- Checkpoint format: structured JSON (machine) + Markdown (human)

### survivaldev-infradoctor

Hook-driven diagnostics and repair for self-hosted Firecrawl and SearXNG instances. Detects failures, diagnoses root causes, applies safe repairs, and validates recovery.

- Autonomous diagnosis → propose fix → safe repair → validate → report loop
- Dispatched automatically on infrastructure incidents

### vibeflow

Single-model Claude Code plugin for conceptualizing, designing, planning, applying, and validating advanced Mistral Vibe workflows. Uses signed intent artifacts, progressive feasibility references, Mermaid/JSON runtime diagrams, and deterministic validation gates.

- Lifecycle: `init → design → plan → apply → validate`
- Init emits signed `VISION.md`, `PLAN.md`, and `WORKFLOW_CONTRACT.json`
- Design maps intent to feasible runtime surfaces instead of assuming impossible middleware/tool/session behavior
- Feasibility substrate covers tiers A-E, key contracts, workflow patterns, events, config keys, tier composition, and observability

### converge

Automates recurring tasks, scheduled workflows, and loop-based execution for AI agents running in CLI environments.

- Cron-based scheduling with natural language support
- Loop execution with self-paced cadence
- Background task management and wake-up calls

### prforge

Delegated PR execution with guarded release, coding discipline enforcement, and distributed mesh mode. Turns the agent into a disciplined upstream contributor.

- Model: investigate → plan → patch → validate → self-review → package → you approve
- Enforces repo intelligence, scope contracts, validation honesty, and git safety
- Distributed mesh mode for multi-repo contribution workflows

## Topics

Browse all plugins by topic: [`claude-code`](https://github.com/topics/claude-code) [`plugin`](https://github.com/topics/plugin) [`survivaldev`](https://github.com/topics/survivaldev)
