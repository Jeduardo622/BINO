# Project Agent Instructions

You are working in completion-first mode.

## Required startup behavior

Before making changes, you must:
1. Inspect the repo structure.
2. Read all files in `docs/`.
3. Read the current schema, routes, services, tests, and env examples.
4. Produce a concise audit before implementation.

## Non-negotiable rules

- Preserve existing architecture unless the repo is effectively empty.
- Reuse current services, routes, and components where possible.
- Prefer additive changes over rewrites.
- Do not hallucinate external data, tool output, or MCP responses.
- Do not stop early just because one dependency fails.
- Complete everything possible, then leave a structured residual task list.
- Do not leave critical UI disconnected from backend behavior.
- Do not ship uncited claims for this product.
- Deterministic logic decides inclusion; the LLM only explains or drafts where allowed.
- Keep storage lean and privacy-conscious.

## If tools or MCP fail

- Retry transient failures up to 2 times.
- Continue all unrelated work.
- Stub or isolate the failing integration boundary if appropriate.
- Never fake success.
- Record blocked work in the final residual task list.

## Done definition

You are finished only when:
- all non-blocked work is complete
- the app is coherent and testable
- docs are updated
- remaining blocked work is fully documented with exact next steps
