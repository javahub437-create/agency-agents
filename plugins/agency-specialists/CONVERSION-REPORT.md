# Conversion report

## Source evidence
- Source repository: https://github.com/msitarzewski/agency-agents
- Source branch: `main`; inspected tree SHA: `4e3ac3ca6604c75113f52c695dbddcc7af928b46`
- The source repository is MIT-licensed.
- Existing Codex integration converts source agents into TOML with name, description, and developer instructions, then installs them to `~/.codex/agents/`.

## Workflow disposition
| Source | Disposition | Reason |
| --- | --- | --- |
| `engineering/engineering-code-reviewer.md` | Compiled into Skill | Evidence-based prioritized review findings. |
| `design/design-ux-researcher.md` | Compiled into Skill | Ethical, evidence-led research plans. |
| `marketing/marketing-content-creator.md` | Compiled into Skill | Audience-focused multi-channel campaign plans. |
| `strategy/runbooks.json` and runbook prose | Compiled into Skill | Phased multi-role plan with dependencies and gates. |
| Codex integration docs and scripts | Reference only | Existing Codex export is a separate distribution surface; scripts can modify local config. |
| Full 230+ agent roster | Reference only | Keep this Plugin curated and avoid hundreds of overlapping Skills. |
| Maintenance CI and contribution workflows | Internal only | Not end-user specialist workflows. |

## Architecture
Skills-only is recommended: the selected workflows primarily encode decision processes, templates, and review standards. A remote MCP server would add deployment, authentication, and privacy obligations without a demonstrated need.

## Validation and limitations
The original local package passed structural checks for manifest JSON/semver, six Skill files with unique names, three SVG assets, safe ZIP paths, clean extraction, and deterministic packaging. Five positive and three negative reviewer scenarios were prepared, but not run as live-host acceptance tests. ChatGPT/Codex live installation and smoke testing were unavailable. The source repository's complete test suite was not run against a full checkout. These checks do not establish OpenAI approval or publication.

## Release boundary
This conversion does not submit to the Plugin Directory, publish a release, or claim approval.