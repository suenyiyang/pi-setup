# Pi Setup

Reusable setup notes for my Pi coding-agent environment.

## How to use this repo

If you are setting up a new computer or a fresh Pi agent environment, you do not need to manually follow every detail in this README. Give this repository, or just this README, to the Pi agent and ask it to restore the setup described here.

For example, you can say:

> Please read this Pi setup README and install the same Pi packages/extensions for me.

The Pi agent should inspect the package list below, install the listed packages, and then verify that they are available.

## Restore selected Pi packages/extensions

On a new computer with Pi installed, give the Pi agent this instruction:

> Install these Pi packages globally for me: `pi-subagents`, `pi-mcp-adapter`, `pi-web-access`, `@juicesharp/rpiv-ask-user-question`, `@plannotator/pi-extension`, `pi-simplify`, `@juicesharp/rpiv-advisor`, `@juicesharp/rpiv-btw`, and `pi-feishu-lark`.

The agent should install each package from npm using `pi install`. Pi currently installs one package at a time, so if a multi-package install fails, ask the agent to install them sequentially.

## Selected packages

| Package | What it does |
|---|---|
| `pi-subagents` | Delegates tasks to subagents with chains, parallel execution, and TUI clarification. |
| `pi-mcp-adapter` | Adds MCP (Model Context Protocol) server/tool integration to Pi. |
| `pi-web-access` | Adds web search, URL fetching, GitHub repo cloning, PDF extraction, YouTube understanding, and local video analysis. |
| `@juicesharp/rpiv-ask-user-question` | Lets the model ask structured, typed questions instead of guessing. |
| `@plannotator/pi-extension` | Supports interactive plan review, annotations, and code/PR review workflows. |
| `pi-simplify` | Reviews recently changed code for clarity, consistency, and maintainability. |
| `@juicesharp/rpiv-advisor` | Lets the model request a second opinion from a stronger reviewer model before acting. |
| `@juicesharp/rpiv-btw` | Adds `/btw` for one-off side questions without polluting the main conversation. |
| `pi-feishu-lark` | Adds Feishu/Lark integration for Pi. |

## Verify installation

After installation, ask the Pi agent to list installed Pi packages and confirm that all packages above are present.

> Note: Pi packages can run code and affect agent behavior. Review third-party package source before installing on a new machine.
