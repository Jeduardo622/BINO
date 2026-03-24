# Cursor + Codex One-Shot Prompt Pack

This pack is designed for Codex running inside Cursor.

It uses a thin controller prompt plus repo docs setup so the agent reads stable project context from files instead of relying on one giant prompt.

## What is included

- `MASTER_PROMPT.md` — the main one-shot prompt you paste into Codex
- `AGENTS.md` — root-level agent instructions for the repo
- `.cursor/rules/00-core-always.mdc` — Cursor project rule, always applied
- `.cursor/rules/10-read-docs-first.mdc` — Cursor project rule to force doc-first behavior
- `docs/PRODUCT.md` — product definition
- `docs/SCOPE.md` — in-scope and out-of-scope boundaries
- `docs/RULES.md` — system rules, safety, privacy, failure handling
- `docs/ARCHITECTURE.md` — preferred architecture and implementation guardrails
- `docs/DATA_MODEL.md` — lean storage and schema guidance
- `docs/ACCEPTANCE.md` — acceptance gates and quality bar
- `docs/RESIDUAL_TASK_TEMPLATE.md` — required final backlog structure
- `docs/VERIFICATION.md` — commands and manual verification checklist

## Recommended use in Cursor

1. Put these files in the project root.
2. Confirm Cursor can see `AGENTS.md` and `.cursor/rules/*`.
3. Open `MASTER_PROMPT.md`.
4. Paste its contents into Codex in Cursor.
5. Attach any additional project files or product memo if needed.

## Why both AGENTS.md and .cursor/rules are included

This pack includes both mechanisms so you have a practical fallback if one is not applied as expected in your environment.

## MCP note

The master prompt includes degraded-mode and residual-task instructions instead of assuming MCP is always available.
