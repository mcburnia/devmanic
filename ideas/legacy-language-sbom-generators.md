# Legacy and Non-Lockfile SBOM Generators

## Problem

Mainstream SBOM generation frequently assumes a package manifest and dependable lockfile. Native, embedded and long-lived software may instead encode dependencies in project files, source includes, compiler commands, linker inputs, maps, bundled code and produced binaries.

The Devmanic opportunity is evidence-based SBOM generation for:

- C and C++;
- Delphi/Object Pascal;
- Fortran;
- Assembly and firmware;
- mixed-language legacy products.

## Shared engine

Build one canonical evidence/component engine with language adapters. Shared capabilities:

- evidence provenance and confidence;
- component identity resolution;
- version and licence resolution;
- PURL/CPE handling;
- dependency relationships;
- user confirmation and exclusion;
- CycloneDX and SPDX output;
- human-readable reports;
- reusable mapping rules.

## Evidence states

- Confirmed
- Declared
- Detected
- Inferred
- User-confirmed
- Excluded

The system must not present inference as confirmed fact.

## C/C++ MVP

Inputs:

- `compile_commands.json`;
- CMake File API output;
- linker map;
- optional ELF/PE/Mach-O binary.

Outputs:

- targets and linked libraries;
- detected component table;
- evidence source and confidence;
- correction workflow;
- CycloneDX JSON.

## Delphi adapter

Inputs may include:

- `.dproj`, `.groupproj`, `.dpk`, `.dpr`;
- Pascal units/includes;
- compiler logs and map files;
- EXE, DLL and BPL artefacts.

Key challenge: map units and directory trees to versioned third-party components while separating RTL/VCL/FMX and first-party code.

## Fortran adapter

Inputs may include:

- CMake/Make/fpm metadata;
- source `USE` and `INCLUDE` relationships;
- compiler dependency output;
- linker commands/maps and produced binaries.

Identify MPI, BLAS/LAPACK, compiler runtimes and mixed-language dependencies.

## Assembly/Firmware adapter

Inputs may include:

- assembler includes;
- object files;
- linker scripts/maps;
- build logs;
- vendor project metadata;
- ELF/PE/firmware images;
- embedded binary blobs and SDK source.

Support dialects incrementally rather than claiming universality.

## Generic workbench

Allow users to review discoveries, merge duplicates, classify first/third-party items, resolve identity/version/licence and save mapping rules for later releases.

## Privacy model

Prefer a free open local scanner that emits a sanitised evidence bundle. Source upload must not be required for commercial/private products.

## Relationship to CRANIS2

Devmanic creates and validates point-in-time SBOMs. CRANIS2 provides continuous regeneration, vulnerability monitoring, licence policy, release history, workflow and retained regulatory evidence.
