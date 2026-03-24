# Architecture

## Preferred architecture if extending an existing repo
- preserve existing architecture
- reuse current services, routes, components, and schema patterns
- prefer additive changes over rewrites

## Preferred architecture if greenfield
- Next.js App Router
- React + TypeScript
- server actions and/or route handlers
- PostgreSQL + Prisma
- simple auth only if needed for save/share
- Vercel-friendly deployment
- minimal background jobs
- OpenAI Responses API only for allowed explanation/drafting tasks

## Technical guardrails
- keep the implementation simple and maintainable
- keep dependencies minimal
- avoid major new subsystems
- keep data models explicit and typed
- keep source normalization compact
- avoid unbounded storage growth

## Allowed LLM usage
- plain-English explanation grounded in retrieved evidence
- outreach draft generation
- bounded normalization assistance only when deterministic parsing is insufficient and uncertainty is preserved

## Forbidden LLM usage
- deciding whether a result exists
- inventing eligibility
- replacing deterministic inclusion logic
- producing uncited surfaced claims
