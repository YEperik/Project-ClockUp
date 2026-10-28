# Roadmap

This roadmap is milestone-driven. A milestone is complete only when its exit criteria are satisfied and evidence is committed.

## Phase 0 — Repository foundation
- [x] Define scope, repository layout, status tracking, and contribution standards.
- [x] Add issue templates and baseline documentation.

## Phase 1 — Reproducible baseline
- [ ] Identify the exact target release and record provenance.
- [ ] Generate a local inventory and cryptographic hashes.
- [ ] Record host OS, analysis tools, versions, and configurations.
- [ ] Define safe local storage conventions for game files.

**Exit criteria:** another researcher can reproduce the inventory and verify the recorded hashes without receiving copyrighted files from this repository.

## Phase 2 — Executable and architecture analysis
- [ ] Identify executable format and target architecture from the binary.
- [ ] Record entry points, memory regions, and relevant loader assumptions.
- [ ] Save a reproducible analysis report.
- [ ] Establish function/address tracking.

**Exit criteria:** conclusions have evidence and confidence labels; uncertain items remain explicitly uncertain.

## Phase 3 — Runtime and file-format mapping
- [ ] Map startup and major runtime paths.
- [ ] Document observed file containers and resource references.
- [ ] Correlate static findings with controlled runtime observations.

**Exit criteria:** at least one subsystem or format is documented with a repeatable validation method.

## Phase 4 — Implementation strategy
- [ ] Compare decompilation, static recompilation, and native reimplementation options.
- [ ] Document hardware-specific dependencies and risk areas.
- [ ] Select an initial proof-of-concept milestone.

**Exit criteria:** decision record identifies rationale, known unknowns, and measurable success criteria.

## Phase 5 — Incremental implementation and validation
- [ ] Implement only behavior supported by analysis.
- [ ] Add regression tests for project-authored code.
- [ ] Maintain checkpoints and a visible list of known gaps.
- [ ] Validate build and runtime behavior independently.

**Exit criteria:** a small end-to-end milestone works and its result can be reproduced.

## Phase 6 — Broader compatibility
- [ ] Expand coverage by subsystem.
- [ ] Track performance, rendering, audio, input, save behavior, and gameplay separately.
- [ ] Publish releases only when the stated capabilities are demonstrably present.

No phase should be marked complete based only on planned work, generated files, or successful compilation.
