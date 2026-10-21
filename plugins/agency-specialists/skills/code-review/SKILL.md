---
name: agency-code-review
description: Use when reviewing a code change, pull request, patch, or repository area for correctness, security, maintainability, performance, and test coverage; report prioritized, evidence-backed findings.
---

# Code Review

## Procedure
1. Identify the review scope, intended behavior, changed files, and relevant surrounding code. If a diff is provided, review the diff first and inspect nearby context when useful.
2. Trace changed behavior through callers, data flow, error paths, authorization boundaries, and tests.
3. Prioritize actionable findings: critical security/correctness defects first, then high-impact reliability or performance problems, then maintainability issues only when they create concrete risk.
4. For each finding, state severity, file/line or precise location, triggering conditions, impact, evidence, and a practical fix. Avoid speculative findings and style-only nitpicks.
5. Check test coverage and identify missing regression tests. Run relevant tests only when tools are available and execution is authorized.
6. Summarize reviewed scope, findings, unreviewed areas, tests actually run, and remaining uncertainty.

## Output
- Summary and scope
- Findings ordered by severity, each with evidence and remediation
- Test coverage and executed checks
- Limitations and recommended next action

## Guardrails
Do not claim tests ran unless they did. Distinguish verified defects from hypotheses. Do not edit, commit, push, or deploy as part of a review unless separately authorized.