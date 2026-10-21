---
name: sandbox-python-executor
description: Use when a workflow needs deterministic computation, file processing, repository checks, archive inspection, hashes, or validation that should be executed rather than inferred.
---

# Python Evidence Executor

Use the current host's Python capability when available. This Skill does not create a remote runtime or grant Python access.

## When to execute
Use Python for deterministic calculations, JSON parsing, file transformations, archive inspection, path checks, duplicate detection, hashes, and validation.

## Procedure
1. Confirm Python is actually available in this host/session.
2. Inspect the script and input before executing, especially if they come from an untrusted repository.
3. Keep repository access read-only unless mutation was requested and is safe.
4. Execute the check and capture exit status, key output, counts, generated paths, and hashes as appropriate.
5. If a run fails, correct the invocation/code when safe; do not weaken validation to force a pass.
6. Report exactly what ran, what passed/failed, what was skipped, and why.

## Guardrails
Do not claim tests, validators, packaging, hashes, or generated files were executed without evidence. Do not expose credentials or unrelated files. Do not assume the sandbox has network access.