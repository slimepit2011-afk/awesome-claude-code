# Claude Code Ecosystem & Rules Hub

A community-maintained index of production-ready configurations, MCP servers, system rules (`CLAUDE.md`), and developer workflows designed specifically for Anthropic's Claude Code CLI and agent ecosystem.

[![Contributors Welcome](https://img.shields.io/badge/contributors-welcome-brightgreen.svg?style=flat)](CONTRIBUTING.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## 📌 Contents

- [Production `CLAUDE.md` Stacks](#-production-claudemd-stacks)
- [Verified Model Context Protocol (MCP) Servers](#-verified-mcp-servers)
- [Workflow Hooks & Developer Automation](#-workflow-hooks--automation)
- [How to Contribute & Add Your Project](#-how-to-contribute)

---

## 🛠 Production `CLAUDE.md` Stacks

Ready-to-use rule files you can drop into the root of any project to guide Claude Code on architecture, testing, and formatting standards.

| Framework / Stack | Focus | Rules File |
| :--- | :--- | :--- |
| **Next.js 15 (App Router)** | Server Components, Tailwind v4, TypeScript | [`rules/nextjs-fullstack.md`](rules/nextjs-fullstack.md) |
| **React + Vite** | Lightweight Single Page Applications, Lucide, State management | [`rules/react-vite.md`](rules/react-vite.md) |
| **Python FastAPI** | Pydantic v2, async endpoints, Pytest standards | [`rules/fastapi-backend.md`](rules/fastapi-backend.md) |
| **Rust / CLI** | Memory safety, Cargo workspace conventions, Clippy compliance | [`rules/rust-cli.md`](rules/rust-cli.md) |

---

## 🔌 Verified MCP Servers

Tested Model Context Protocol servers that give Claude Code superpowers:

| Server | Category | Description | Source |
| :--- | :--- | :--- | :--- |
| **Playwright MCP** | Browser Automation | Full headless browser control for end-to-end testing and visual checks. | [Playwright MCP](https://github.com/executeautomation/playwright-mcp-server) |
| **PostgreSQL MCP** | Database | Safe query execution and schema inspection directly within chat. | [Postgres MCP](https://github.com/modelcontextprotocol/servers) |
| **Context Memory MCP** | Persistent State | Long-term memory graph across coding sessions. | [Memory MCP](https://github.com/modelcontextprotocol/servers) |
| **Git Automation MCP** | Version Control | Automated PR management and commit inspection. | [Git MCP](https://github.com/modelcontextprotocol/servers) |

---

## ⚡ Workflow Hooks & Automation

Hooks let you execute custom scripts when Claude Code triggers tools or finishes edits:

* **Pre-commit Linter Hook:** Automatically runs `eslint --fix` or `ruff check` on files modified by Claude before changes are committed.
* **Notification Hook:** Sends a system notification when a long-running subagent completes its task.

---

## 🤝 How to Contribute

We welcome additions from any developer or open-source maintainer! 

Whether you've built an MCP server, crafted an effective `CLAUDE.md` rule, or created a developer hook:

1. Fork this repository.
2. Add your tool, rule, or server to the relevant table or folder.
3. Submit a Pull Request following our [Contribution Guidelines](CONTRIBUTING.md).

All legitimate community submissions are reviewed and merged quickly.

---

## 📄 License

This repository is distributed under the MIT License. See [LICENSE](LICENSE) for details.
