# Copilot instructions — ghcp-for-mainframe

This repository is a [MoaW](https://moaw.dev) workshop: **GitHub Copilot for Mainframe Modernization**. It contains documentation only.

- The workshop is a single file: `docs/workshop.md`. Images live in `docs/assets/` and are referenced as `assets/<name>`.
- Keep the MoaW format: YAML frontmatter at the top, `---` separates pages, and every page starts with the same `<style>…</style>` line. Callouts use `<div class="info|tip|warning" data-title="…">` with a blank line and `> ` quoted content inside.
- Chapters: 1 = Getting Started (1.1–1.8), 2 = Mainframe App Modernization (2.1–2.7). Keep section numbers in headings consistent when adding or moving sections.
- All hands-on material (agents, prompts, skills, copilot-instructions) lives in the fork [jkordick/Bank-of-Z](https://github.com/jkordick/Bank-of-Z), not here. When the workshop text names an agent, prompt, skill, file path or number (e.g. "39 of 44 programs parsed"), it must match that fork.
- Mark data-layer topics (DB2, IMS DB, VSAM, data migration) with 🗄️.
- Add an "In the Copilot CLI:" note when a VS Code instruction behaves differently in the CLI.
