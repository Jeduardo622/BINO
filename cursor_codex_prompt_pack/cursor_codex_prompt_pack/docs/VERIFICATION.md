# Verification

## Verification order
1. Inspect repo scripts and use the real commands if they exist.
2. Run the smallest relevant checks first.
3. Then run broader project checks.

## Typical command order
- install dependencies
- generate client/codegen if needed
- run migrations if applicable
- typecheck
- lint
- targeted tests
- full tests if practical
- build
- local run sanity check if feasible

## Manual checks
- complete intake flow
- submit a valid profile
- confirm result generation works
- confirm every surfaced result has citation + source link + last checked state
- confirm unknown fields are shown as unknown
- confirm outreach draft is optional and editable
- confirm save/share works according to the chosen auth/session model
- confirm error and empty states render correctly
- confirm privacy/safety copy is visible

## Reporting rule
If any verification step cannot be executed, document:
- the exact blocker
- what was tried
- what fallback was used
- what remains to verify
