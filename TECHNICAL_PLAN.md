# BOMGuard - technical plan

**Planning document, not an implementation report.**

## Product objective

Electrical-design-aware comparisons with explicit substitution and metadata rules.

## Intended system boundary

- **Input:** Invented resistor/capacitor/controller BOMs created as test fixtures.
- **Processing stages:** KiCad/CSV import adapters; Normalized component identity model; Policy-driven comparison engine; CLI and report writers.
- **Output:** A sample change report clearly identifies high-impact differences.
- **Runtime / build stack (tentative):** Python 3.12+, Typer, CSV, KiCad export adapters, pytest
- **Explicitly excluded:** Supply-chain procurement transactions, real pricing/financial records, or access to confidential customer designs.

## Functional modules

- Import standard KiCad-compatible CSV BOM exports
- Normalize references, values, footprints, and manufacturer part numbers
- Detect additions, deletions, value changes, and possible substitutions
- Apply configurable component equivalence policies and flag uncertainties
- Output human-readable Markdown and machine-readable JSON diffs

## Demonstration and acceptance cases

**Test 1:** Compare two synthetic PCB revisions and find footprint changes

**Test 2:** Flag an apparent substitution requiring human review

**Test 3:** Generate a release summary suitable for an open-hardware changelog

## Safety, privacy, and provenance

1. Keep example datasets fictional, self-created, or appropriately licensed.
2. Run locally for the initial prototype; do not collect data on actual third parties.
3. Document origin and versions of external specifications and dependencies.
4. Exclude production credentials; put environment variable *names* only in `.env.example` if required later.
5. Do not make certification, legal compliance, professional safety, or performance guarantees without independent validation.

## Engineering unknowns and constraints

Equivalence is contextual and may be unsafe to infer; require explicit review of potential substitutes.

## Release definition

A first release requires a runnable prototype, verified README instructions, automated tests tied to the three demonstrations, the full LICENSE file, and an honest public GitHub development history. The roadmap estimates are hypotheses until reviewed during implementation.
