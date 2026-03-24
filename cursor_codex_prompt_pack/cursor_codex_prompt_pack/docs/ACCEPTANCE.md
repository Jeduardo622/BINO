# Acceptance

## Critical acceptance gates

### 1. Schema gate
- database schema exists and supports the real MVP flow
- migrations are present
- persistence is real, not mock-only

### 2. Backend gate
- core routes/services work with real data or clearly isolated fallbacks
- validation and error handling exist
- citations and canonical links are enforced

### 3. Frontend integration gate
- UI is wired to backend behavior
- intake, results, save/share, and draft generation flows are functional
- loading / empty / error states exist

### 4. Safety framing gate
- navigation, not medical advice
- preliminary eligibility language only
- uncertainty is surfaced
- verify-with-site language is visible

### 5. Deterministic logic gate
- inclusion/filtering is explainable and testable
- freeform LLM behavior does not decide inclusion

### 6. Citation gate
- every surfaced result has source backing and canonical links
- no uncited eligibility claims are allowed through

### 7. Privacy gate
- only necessary data is stored
- retention is minimal
- deletion/removal support exists if practical or is clearly documented as deferred

### 8. UX gate
- the product feels coherent and usable
- critical screens are not placeholders

### 9. Testing gate
- focused tests exist for fragile and critical logic
- core commands pass or failures are honestly documented

### 10. Build gate
- app builds
- migrations are runnable
- setup instructions are sufficient for another engineer to run the app

## MVP quality bar
- parents can get to 3 to 5 usable options
- surfaced results are citation-backed
- contact paths are visible when available
- flow supports review in under 10 minutes
