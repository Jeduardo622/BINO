# Rules

## Core product principles
- Retrieval is the source of truth.
- Deterministic filters decide inclusion where fields exist.
- The LLM may explain or draft, but it does not decide truth.
- No surfaced result without citation and canonical source link.
- No uncited eligibility claim.
- Unknown fields must remain unknown.

## Safety and UX framing
Use language like:
- potential match
- preliminary fit
- what to verify
- verify with coordinator or program staff
- source
- last checked
- unknown / not stated by source

Avoid language like:
- best match
- guaranteed eligibility
- recommended treatment
- AI diagnosis
- you qualify

## Privacy
- Store the minimum child profile data required for the workflow.
- Avoid unnecessary sensitive identifiers.
- Keep retention lean.
- Add deletion/removal support if practical.
- Do not claim compliance levels that the implementation does not actually satisfy.

## Cost and complexity
- Prefer deterministic code over LLM usage.
- Keep LLM calls bounded and purposeful.
- Keep expensive generation on-demand.
- Avoid broad scraping.
- Avoid always-on browser automation.
- Avoid heavy new infrastructure unless clearly necessary.

## Failure handling
If an external dependency fails:
- retry up to 2 times if reasonable
- continue all other work
- isolate or stub the failing boundary if appropriate
- never fake success
- record blocked work in the residual task list
