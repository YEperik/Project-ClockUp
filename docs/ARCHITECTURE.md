# Architecture Notes

## Current state

This is a documentation and workspace scaffold. No executable architecture, recovered code layout, or native runtime architecture has been verified yet.

## Intended separation of concerns

- **Reverse-engineering evidence:** analysis notes, addresses, symbol maps, and file-format research.
- **Decompilation artifacts:** recovered or reconstructed code, with original address mapping and confidence labels.
- **Native PC experiments:** host-side code and platform abstractions, kept separate from unverified reverse-engineering notes.
- **Tools:** project-authored utilities for repeatability and validation.
- **Tests:** automated checks for tools and recovered behavior.
- **Checkpoints:** text manifests recording commit, tool versions, target hashes, known gaps, and next verified milestone.

## Architecture decision records

When a consequential technical choice is made, add a short record under `docs/decisions/` containing:

1. Context and constraints.
2. Options considered.
3. Decision and rationale.
4. Evidence and assumptions.
5. Consequences, risks, and conditions that would trigger reconsideration.

Do not add guessed details to this document. Update it as verified findings emerge.
