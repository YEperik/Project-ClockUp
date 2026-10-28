# Technical Approach

## Purpose

This document defines a cautious workflow for understanding the PlayStation 2 version of _Kamen Rider Kabuto_ and assessing possible routes toward a native PC implementation.

## Terminology

- **Disassembly:** translating machine instructions into assembly-language representations.
- **Decompilation:** recovering higher-level source-like representations from machine code. Results require validation and are not automatically equivalent to original source.
- **Asset extraction:** locating and decoding resources such as models, textures, audio, and archives. This does not decompile game logic.
- **Static recompilation:** translating machine-code behavior into code that can execute on another host while attempting to preserve behavior.
- **Native reimplementation:** rebuilding systems in a host-native architecture using recovered behavior and data formats.
- **Emulation:** reproducing hardware behavior in software. It is useful for comparison but is not itself a native port.

## Analysis stages

### 1. Baseline and provenance

Record the exact game release identifier, source of the analysis copy, file inventory, hashes, tool versions, and host environment. Keep game data outside the public repository.

### 2. Executable identification

Determine the executable format, target processor and ABI, load addresses, entry points, code/data boundaries, and available symbol or relocation information. Do not infer a property solely from the filename.

### 3. Static analysis

Create an analysis database and maintain a stable ledger of function addresses, candidate names, callers/callees, data references, and confidence. Preserve address mapping between original machine code and any exported representations.

### 4. Dynamic observation

Where legally and technically appropriate, compare static hypotheses with repeatable runtime observations. Record the emulator or hardware environment, configuration, test inputs, and expected/observed results.

### 5. Subsystem research

Investigate systems as evidence allows, potentially including startup, memory layout, file I/O, rendering, animation, audio, controller input, battle logic, UI, and saves. Do not assume the implementation details before analysis.

### 6. Strategy decision

Evaluate function-level decompilation, static recompilation, and native reimplementation against the actual executable, dependencies, hardware-specific behavior, testability, and maintenance cost. The chosen path may be hybrid, but the decision must be documented.

### 7. Validation

Prefer small, measurable milestones. Compare observable behavior and outputs. Record failures and limitations instead of masking them. Track separate states for analysis completion, build success, and runtime compatibility.

## Tooling candidates

Tools are selected based on evidence and compatibility rather than treated as mandatory:

- Ghidra with an appropriate MIPS/PS2 analysis configuration for static analysis.
- A trusted PS2 emulator or original hardware for behavioral comparison.
- Compiler/build tools such as CMake and a C++ toolchain if native code is introduced.
- Project-authored scripts for repeatable inventory, hashing, symbol export, and validation.

Tool support does not guarantee a correct result. Tool versions and relevant configuration must be recorded.
