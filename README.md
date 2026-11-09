# Power Automate skill for GitHub Copilot

This repository contains a repository-scoped GitHub Copilot skill at:

```text
.github/skills/power-automate/SKILL.md
```

The skill guides Copilot through planning, validating, and safely managing Power Automate cloud flows. It does not install the Power Automate plugin, provide FlowAgent tools, sign in to Microsoft, or grant access to an environment.

## Use in this repository

Open this repository in a GitHub Copilot experience that supports repository skills. Copilot can use the skill instructions when working in this repository.

## Use Power Automate tools

For actual flow operations, use a client with FlowAgent MCP tools. In GitHub Copilot CLI, the Microsoft plugin can be installed with:

```text
/plugin marketplace add microsoft/power-platform-skills
/plugin install power-automate@power-platform-skills
```

FlowAgent also requires Node.js and Microsoft authentication through Azure CLI. Sign in on the same machine and user account where Copilot CLI runs:

```bash
az login
```

Authentication and permissions are independent of this repository skill. Never commit credentials, access tokens, or authentication caches.
