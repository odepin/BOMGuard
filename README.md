# BOMGuard

> Meaningful bill-of-materials diffs for electronics projects.

**Current state:** Documentation starter / proposed product. The presence of this README does **not** mean the software has been implemented, deployed, used. Update this status to reflect real work.

## What it is

BOMGuard is a proposed specialist software tool for KiCad users, hardware startups working on non-confidential demos, and open-hardware maintainers. Spreadsheet diffs miss engineering significance when components are renamed, substituted, or reorganized. The intended differentiation is: Electrical-design-aware comparisons with explicit substitution and metadata rules.

## Intended users and use cases

- Compare two synthetic PCB revisions and find footprint changes
- Flag an apparent substitution requiring human review
- Generate a release summary suitable for an open-hardware changelog

## Planned features

- Import standard KiCad-compatible CSV BOM exports
- Normalize references, values, footprints, and manufacturer part numbers
- Detect additions, deletions, value changes, and possible substitutions
- Apply configurable component equivalence policies and flag uncertainties
- Output human-readable Markdown and machine-readable JSON diffs

## Proposed technology

Python 3.12+, Typer, CSV, KiCad export adapters, pytest

These technologies are *planned*, not a claim that dependencies have already been installed or code has been written. Revise this section when actual implementation decisions are made.

## Proposed architecture

- KiCad/CSV import adapters
- Normalized component identity model
- Policy-driven comparison engine
- CLI and report writers

See [TECHNICAL_PLAN.md](TECHNICAL_PLAN.md) for technical boundaries and acceptance tests.

## Running locally

**Not yet runnable.** This package contains documentation templates, not software. When a functioning implementation is available, replace this paragraph with tested prerequisites, install instructions, a verified executable command, and a reproducible example using `Invented resistor/capacitor/controller BOMs created as test fixtures.`

## Data boundaries and exclusions

Supply-chain procurement transactions, real pricing/financial records, or access to confidential customer designs. All public examples should use Invented resistor/capacitor/controller BOMs created as test fixtures.

## Known limitations / validation risks

Equivalence is contextual and may be unsafe to infer; require explicit review of potential substitutes.

## Development roadmap

Work is broken into estimated, not-yet-completed milestones in [ROADMAP.md](ROADMAP.md). They are *planning estimates*, not an assertion that development has begun or that work will definitely be performed.

## Business direction

Potential commercial extensions: Professional release checks, PLM connectors, and advanced rule packs. 

## Contributing and licensing

License: [Mozilla Public License 2.0](LICENSE) (`MPL-2.0`). The distribution contains the complete license text. Any future source files can include the SPDX identifier `MPL-2.0` and the Exhibit A notice where appropriate. Rights in contributions and project ownership must be verified before licensing.

