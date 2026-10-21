---
name: host-workspace-operator
description: Use when inspecting or changing repository files, diagnosing failures, or operating on a host workspace; prefer read/search-first, minimal changes, and explicit verification.
---

# Host Workspace Operator

## Procedure
1. Confirm the requested outcome, workspace/repository, constraints, and permitted mutation scope.
2. Inspect available tools and permissions before choosing a workflow; never assume shell, network, or write access exists.
3. Start read-only: list relevant files, search for symbols/errors, inspect status and nearby context.
4. Form a short hypothesis and gather evidence before editing. Avoid broad scans of unrelated or sensitive files.
5. Propose the smallest coherent change. Preserve existing conventions and avoid unrelated formatting or refactors.
6. Before mutating files or running commands with side effects, ensure the user authorized that class of change. Never expose credentials or secrets.
7. Apply the change with the safest available editor/patch tool. Review the diff for scope and accidental changes.
8. Run targeted tests, linters, or checks when available and authorized; record exact commands and results.
9. Summarize changed files, verification, limitations, and rollback considerations.

## Guardrails
Do not claim unavailable tools were used. Avoid destructive operations, force pushes, production changes, or broad deletion without explicit authorization.