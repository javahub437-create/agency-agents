# Agency Specialists for ChatGPT Desktop (Local Marketplace)

This folder packages four skills as a starter plugin: code review, UX research planning, content campaign planning, and project runbook orchestration.

## Install locally

1. Clone this repository to your computer, or pull the branch containing this configuration.
2. Open the repository root in the ChatGPT desktop app's supported local-workflow environment.
3. Restart ChatGPT desktop after adding or changing the marketplace.
4. Open the Plugins Directory, select **Agency Specialists (Local)**, and install **Agency Specialists**.
5. Open a new chat and try one of the starter prompts. Confirm the plugin appears and that each skill is available.

The marketplace is defined at `.agents/plugins/marketplace.json`; it references this plugin using the repository-relative path `./plugins/agency-specialists`.

## Scope and limitations

This is a skills-only starter plugin. It does not add an MCP server, external account connection, or grant access to GitHub or other services. Skills provide reusable instructions; actual repository operations require compatible tools and user permissions.

The GitHub repository itself is not a local filesystem installation. Clone or otherwise make the repository available locally before using this repo-scoped marketplace in the desktop app.

## Validation

Validate the marketplace and plugin manifest as JSON, confirm all referenced skill files exist, then restart the desktop app and verify the plugin in the Plugins Directory. No installation is considered complete until the desktop app confirms it.
