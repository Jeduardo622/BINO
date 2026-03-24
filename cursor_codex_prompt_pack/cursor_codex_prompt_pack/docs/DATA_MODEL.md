# Data Model

## Core entities
- User or Session
- Profile (child intake)
- SourceRecord (normalized trial or program)
- MatchResult or computed result layer
- SavedItem
- Share artifact if needed
- Review / QA record if needed
- Generated outreach draft if persisted

## Store only what is needed for
- intake-to-result workflow
- filtering and ranking
- citation-backed explanation
- source verification
- save/share
- lightweight review support

## Compact retained fields
- source
- source record ID
- title or program name
- organization or center name
- normalized condition tags
- age range if available
- location if available
- recruitment/availability status if applicable
- relevant dates
- short summary or excerpt
- canonical source URL
- contact path fields if directly available
- source timestamps / last checked
- deterministic fit flags or normalized fields

## Do not store by default
- mirrored full documents
- unnecessary child identifiers
- unlimited raw payload history
- broad raw dumps
- unsupported inferred facts
- large attachment copies

## Qualified match definition
A qualified match is a result where:
- source is credible
- freshness is shown or recent enough
- age and condition broadly align where data exists
- exclusions or unknowns are surfaced
- canonical verification link is present
- a contact path or practical next step is present or marked missing
- explanation is citation-backed
- claims do not exceed the evidence
