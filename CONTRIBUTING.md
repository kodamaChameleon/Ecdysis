# Ecdysis Contributing Guide

Thank you for taking an interest in Ecdysis. Contributions that improve compatibility with new Obsidian releases, fix visual regressions, or refine existing styling are welcome. New features or significant design changes should be discussed in an issue before a pull request is opened.

---

## Reporting Issues

Before opening a new issue, please search existing issues to avoid duplicates.

When reporting a bug, include:

- Obsidian version
- Operating system
- Ecdysis version (from `manifest.json`)
- Steps to reproduce the problem
- Whether the issue persists when all other CSS snippets are disabled
- A screenshot if the issue is visual

---

## Submitting Pull Requests

1. Fork the repository and branch from `master`
2. Edit `theme.css` directly — there is no SCSS build step or generated file
3. Keep pull requests focused on a single fix or change; avoid unrelated cleanup in the same PR
4. Open the PR with a clear description of what changed and why

When editing `theme.css`, follow the existing conventions:

- Colors are referenced through palette variables (`--clr-green`, `--clr-cyan`, etc.) rather than hardcoded hex values wherever possible
- Hardcoded `rgba()` values are acceptable where CSS variables cannot be used (e.g. callout color overrides)
- Sections are separated by the established block comment style
- Comments explain *why* something is done when the reason is non-obvious (e.g. Obsidian cascade quirks)

---

## Improving Documentation

Updates to `README.md` or `CONTRIBUTING.md` are welcome via pull request. If you notice that documented behavior no longer matches the theme, please open an issue or submit a correction directly.
