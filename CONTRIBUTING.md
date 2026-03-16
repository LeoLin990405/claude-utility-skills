# Contributing to Claude Utility Skills

Thank you for your interest in contributing! This document provides guidelines for contributing to this repository.

## How to Contribute

### Reporting Bugs

1. Check existing [issues](https://github.com/LeoLin990405/claude-utility-skills/issues) to avoid duplicates.
2. Open a new issue using the **Bug Report** template.
3. Include steps to reproduce, expected behavior, and actual behavior.

### Requesting Features

1. Open a new issue using the **Feature Request** template.
2. Describe the use case and why this feature would be valuable.

### Submitting a New Skill

1. Fork the repository and create a feature branch.
2. Use the `skill-creator` skill or scaffold manually:
   ```bash
   python skills/skill-creator/scripts/init_skill.py <skill-name>
   ```
3. Place your skill under `skills/<skill-name>/`.
4. Every skill **must** include a `SKILL.md` with valid YAML frontmatter:
   ```yaml
   ---
   name: your-skill-name
   description: One-line description
   version: 1.0.0
   ---
   ```
5. Add a brief entry to the root `SKILL.md` index.
6. Submit a pull request following the PR template.

### Improving Existing Skills

- Fix typos, improve documentation, add examples -- all welcome.
- For significant changes, open an issue first to discuss the approach.

## Skill Quality Checklist

Before submitting, verify your skill meets these criteria:

- [ ] `SKILL.md` has valid YAML frontmatter (`name`, `description`, `version`)
- [ ] Clear, actionable instructions in the skill body
- [ ] Examples or references included where appropriate
- [ ] No hardcoded paths or credentials
- [ ] Tested with Claude Code locally

## Code Style

- Markdown: Use ATX-style headers (`#`), fenced code blocks with language tags.
- Python scripts: Follow PEP 8. Include docstrings for public functions.
- File names: Use lowercase with hyphens (`my-skill`, not `MySkill` or `my_skill`).

## Pull Request Process

1. Ensure your branch is up to date with `main`.
2. Fill out the PR template completely.
3. Wait for review -- PRs are reviewed by maintainers and Claude Code review action.
4. Address any feedback and push updates to the same branch.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
