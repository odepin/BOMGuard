# BOMGuard - development roadmap

**Status:** Planned work only. None of the boxes are marked completed. Estimates are rough.

## Product-level acceptance criterion

A sample change report clearly identifies high-impact differences.

## Estimated work breakdown

| Step | Milestone | Estimated hours | Observable outcome |
|---|---|---:|---|
| 1 | Design normalized BOM structure | 7 | Typed schema with controlled field names |
| 2 | Implement CSV/KiCad import | 9 | Fixtures import with stable IDs |
| 3 | Build semantic diff rules | 11 | Tests distinguish meaningful vs cosmetic changes |
| 4 | Create equivalence-policy engine | 8 | Unsafe assumptions surface as warnings |
| 5 | Develop CLI and report formats | 8 | Useful release notes from sample BOMs |
| 6 | Tests and documentation | 9 | CI validates fixture comparisons |
| | **Total estimated** | **52** | |

## Detailed milestones

### 1. Design normalized BOM structure (7 estimated hours)

- [ ] Deliverable: Typed schema with controlled field names.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 2. Implement CSV/KiCad import (9 estimated hours)

- [ ] Deliverable: Fixtures import with stable IDs.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 3. Build semantic diff rules (11 estimated hours)

- [ ] Deliverable: Tests distinguish meaningful vs cosmetic changes.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 4. Create equivalence-policy engine (8 estimated hours)

- [ ] Deliverable: Unsafe assumptions surface as warnings.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 5. Develop CLI and report formats (8 estimated hours)

- [ ] Deliverable: Useful release notes from sample BOMs.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 6. Tests and documentation (9 estimated hours)

- [ ] Deliverable: CI validates fixture comparisons.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

## QA and release gates

- [ ] A real runnable implementation exists, with verified setup commands in `README.md`.
- [ ] Automated tests pass in a clean environment and failures are actionable.
- [ ] Only fabricated, original, openly licensed, or otherwise authorized sample data is published.
- [ ] No passwords, API keys, secrets, customer records, or employer/client confidential artifacts appear in repository history.
- [ ] A source-linked change log and actual progress notes distinguish finished work from plans.
- [ ] The GitHub history preserves authentic work and authorship; do **not** manufacture or backdate commits.

## Parking lot and risks

- Technical: Equivalence is contextual and may be unsafe to infer; require explicit review of potential substitutes.
- Commercial hypothesis (not validated): Professional release checks, PLM connectors, and advanced rule packs.
- Beyond MVP: defer paid extensions and hosted features until the underlying product works.
