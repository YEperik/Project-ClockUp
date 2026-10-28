# Contributing

Thank you for helping improve the technical quality of this project. Contributions should make the work more reproducible, more accurate, or easier to validate.

## Ground rules

1. **Evidence over confidence.** Include the observations that support a conclusion.
2. **No fabricated behavior.** Do not add dummy implementations, invented structures, false success results, or unverified compatibility claims.
3. **Keep changes reviewable.** Prefer small commits with one clear purpose.
4. **Preserve provenance.** Record tool versions, relevant settings, addresses, hashes, and reproducible commands when applicable.
5. **Protect copyrighted material.** Do not submit disc images, game executables, extracted assets, or other material that you are not authorized to redistribute.
6. **Separate fact from interpretation.** Label findings Confirmed, Strongly supported, Hypothesis, Unknown, or Blocked.

## Research note format

For significant reverse-engineering findings, include:

- **Question:** What are you trying to determine?
- **Target:** File identifier/hash and address or offset range, where applicable.
- **Environment:** Tool name/version and relevant settings.
- **Method:** Steps or commands required to reproduce the observation.
- **Observation:** What was actually seen.
- **Interpretation:** What the observation may mean.
- **Confidence:** One of the project confidence labels.
- **Open questions:** What remains unverified.
- **Evidence:** Safe-to-share logs, screenshots, pseudocode, or small excerpts where lawful.

## Code standards

- Avoid unrelated refactors in analysis commits.
- Add tests for project-authored parsers, utilities, and recovered behavior where feasible.
- Do not label guessed pseudocode as recovered source.
- Keep tool output and generated artifacts deterministic where possible.
- Never commit secrets, personal paths, proprietary files, or large binary dumps.

## Pull requests

A pull request should state:

- What changed and why.
- How it was tested.
- What evidence supports any new technical claim.
- Known limitations or unresolved issues.
- Whether `PROJECT_STATUS.md` and `CHANGELOG.md` need updates.

A clean build is not the same as a successful runtime test. State exactly what was verified.
