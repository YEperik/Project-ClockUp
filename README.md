<div align="center">
<img src="assets/social-preview.png" alt="Kamen Rider Kabuto PS2 Decompilation Project banner" width="100%">

# Kamen Rider Kabuto — PS2 Decompilation Project

**Reverse engineering · executable analysis · decompilation research · native PC feasibility**

[![Platform](https://img.shields.io/badge/platform-PlayStation%202-161b22?style=for-the-badge)](#target) [![Status](https://img.shields.io/badge/status-foundation%20phase-c9a34a?style=for-the-badge)](PROJECT_STATUS.md) [![Research](https://img.shields.io/badge/research-evidence--driven-8b1e2d?style=for-the-badge)](docs/TECHNICAL_APPROACH.md)
</div>

> **Mission:** reconstruct a reliable technical understanding of the PlayStation 2 release of *Kamen Rider Kabuto*, document executable and runtime systems with reproducible evidence, and determine a sound path toward a native PC implementation.

## Overview

*Kamen Rider Kabuto* is a PlayStation 2 action-fighting game released in Japan in 2006. This repository is the engineering workspace for studying its executable, program behavior, data formats, and platform-specific systems.

The project keeps analysis evidence, reconstructed code, implementation experiments, and validation separate. Every claimed milestone must have evidence; unverified behavior remains explicitly unverified.

## Project principles

- **Evidence before assumptions** — technical claims must be reproducible or labeled as hypotheses.
- **Small, verifiable milestones** — make progress measurable and regressions easier to isolate.
- **No fake completion** — no empty stubs, hardcoded success results, or invented test reports presented as real functionality.
- **Analysis is not implementation** — disassembly, decompilation, asset research, emulation, and native reimplementation are tracked separately.
- **Preserve the original** — keep game data and proprietary binaries out of public Git history.
- **Build for maintainability** — document tools, addresses, evidence, decisions, blockers, and checkpoints.

## Target

| Field | Details |
|---|---|
| Title | Kamen Rider Kabuto (仮面ライダーカブト) |
| Platform | PlayStation 2 |
| Region | Japan (NTSC-J) |
| Product code | `SLPS-20483` |
| Original release | 30 November 2006 |
| Developer | Digifloyd |
| Publisher | Bandai Namco Games |
| Long-term objective | Evaluate and, if feasible, develop a native PC implementation |

Metadata identifies the target release. This is an independent fan research project and is not affiliated with or endorsed by the rights holders.

## Current status

**Foundation phase.** Repository structure, documentation, issue templates, and visual identity are established. Executable analysis has not yet been recorded here, and no completed decompilation, native PC build, or compatibility result is claimed.

See [Project Status](PROJECT_STATUS.md) and the [Roadmap](docs/ROADMAP.md).

## Repository map

```text
.
├── assets/                   # Project-authored repository artwork
├── docs/                     # Technical approach, roadmap, architecture, glossary
├── reverse_engineering/      # Analysis, Ghidra workflow, symbols, formats
├── decompilation/            # Reconstructed source, types, validation tests
├── native_pc/                # Native implementation experiments
├── tools/                    # Project-authored analysis and validation tools
├── tests/                    # Repository-level tests
├── checkpoints/              # Reproducibility manifests
├── .github/                  # Issue templates and PR checklist
├── PROJECT_STATUS.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── CITATION.cff
├── LICENSE
└── SECURITY.md
```

Directories are scaffolding until verified work exists inside them; their presence is not a claim that a feature is implemented.

## Engineering workflow

1. **Baseline the target.** Record release identity, local file inventory, hashes, tool versions, and analysis environment.
2. **Identify the executable.** Determine format, architecture, entry points, memory regions, and code/data boundaries from evidence.
3. **Map program behavior.** Track functions, references, calling conventions, structures, and confidence without losing original addresses.
4. **Investigate runtime systems.** Compare static findings with controlled observations where appropriate.
5. **Choose an implementation strategy.** Evaluate decompilation, static recompilation, and native reimplementation based on findings—not assumptions.
6. **Validate continuously.** Separate successful analysis, compilation, and demonstrated runtime compatibility.
7. **Checkpoint progress.** Record commit, tool versions, verified results, known gaps, and next reproducible action.

## Finding confidence

| Label | Meaning |
|---|---|
| **Confirmed** | Directly supported by reproducible evidence. |
| **Strongly supported** | Multiple independent observations support the conclusion. |
| **Hypothesis** | Plausible interpretation that still requires testing. |
| **Unknown** | Evidence is insufficient to reach a conclusion. |
| **Blocked** | Progress depends on resolving a documented blocker. |

## Getting started

This is currently a research scaffold, not a runnable game or port. Read [Project Status](PROJECT_STATUS.md), follow the [Technical Approach](docs/TECHNICAL_APPROACH.md), review the [Roadmap](docs/ROADMAP.md), and follow [Contribution and Evidence Standards](CONTRIBUTING.md). Keep disc images, game executables, extracted assets, and proprietary dumps outside this repository.

## Legal and distribution

This project is intended for software research, interoperability, and technical documentation. Do not commit disc images, game executables, extracted copyrighted assets, or materials you are not authorized to redistribute.

The repository license covers only original project-authored material. It does not grant rights to the game, its code, characters, artwork, trademarks, or other third-party intellectual property.

## Search keywords

Kamen Rider Kabuto, 仮面ライダーカブト, PS2, PlayStation 2, SLPS-20483, reverse engineering, decompilation, MIPS, Ghidra, game preservation, native PC port.
