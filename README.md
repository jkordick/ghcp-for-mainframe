# GitHub Copilot for Mainframe Modernization

**A hands-on GitHub Copilot workshop for mainframe application modernization — COBOL, CICS, DB2, IMS and batch — on IBM's [Bank of Z](https://github.com/IBM/Bank-of-Z).**

This is a [MoaW](https://moaw.dev) workshop. The best way to read it is rendered:

👉 **[Open the workshop on MoaW](https://moaw.dev/workshop/gh:jkordick/ghcp-for-mainframe/main/docs/)**

Or read the raw markdown: [`docs/workshop.md`](docs/workshop.md).

## What you'll learn

1. **Getting Started with GitHub Copilot** — inline completions, Chat, Agent mode, the Copilot CLI, custom instructions, prompt files, custom agents, skills and MCP servers, all on real COBOL.
2. **Mainframe App Modernization** — a four-phase, agentic modernization (rediscovery → substitution audit → re-architecture / re-write → deployment) driven by custom agents and prompt files, with a deterministic [cobol-rekt](https://github.com/avishek-sen-gupta/cobol-rekt) *source of truth* that every LLM-written claim is cross-checked against.

## Where the hands-on material lives

This repository contains only the workshop text. Everything you run lives in the workshop fork of Bank of Z:

👉 **[jkordick/Bank-of-Z](https://github.com/jkordick/Bank-of-Z)** — IBM's Bank of Z plus a `.github/` kit:

| Path | Content |
| --- | --- |
| `.github/copilot-instructions.md` | Bank of Z layout, COBOL conventions, work rules |
| `.github/agents/` | `cobol-archaeologist`, `substitution-auditor`, `target-architect`, `module-rewriter`, `deployment-engineer` |
| `.github/prompts/` | 14 phase prompts (`01-rediscovery-*` … `04-deploy-*`) |
| `.github/skills/` | `cobol-rekt` (source of truth), `cobol-dependency-scan`, `copybook-resolver` |

## Pre-reqs

- A GitHub account with Copilot access (Free, Pro, Business or Enterprise)
- VS Code with the GitHub Copilot + Copilot Chat extensions (IBM Z Open Editor optional). Chats must use the **Local** agent harness, because the default Copilot harness doesn't load prompt files (see workshop 1.1).
- Java 21+ and Python 3.9+ (for the cobol-rekt source of truth)
- GitHub CLI (`gh`) and the GitHub Copilot CLI
- bash / zsh (Git Bash or WSL on Windows)
- A fork of [jkordick/Bank-of-Z](https://github.com/jkordick/Bank-of-Z/fork)

No mainframe access is required. See [the Pre-requisites section of the workshop](docs/workshop.md#pre-requisites) for details.

## License

MIT — see [LICENSE](LICENSE). Bank of Z and cobol-rekt are licensed by their respective owners.

## Credits

- Based on [GitHub Copilot Advanced](https://moaw.dev/workshop/gh:jkordick/ghcp-advanced/main/docs/) ([repo](https://github.com/jkordick/ghcp-advanced)).
- [Bank of Z](https://github.com/IBM/Bank-of-Z) by IBM.
- [cobol-rekt](https://github.com/avishek-sen-gupta/cobol-rekt) by Avishek Sen Gupta.
