<p align="center">
  <img src="https://img.shields.io/github/license/LeoLin990405/claude-utility-skills?style=flat-square" alt="License">
  <img src="https://img.shields.io/github/stars/LeoLin990405/claude-utility-skills?style=flat-square" alt="Stars">
  <img src="https://img.shields.io/github/issues/LeoLin990405/claude-utility-skills?style=flat-square" alt="Issues">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-8A2BE2?style=flat-square&logo=anthropic&logoColor=white" alt="Claude Code Skill">
</p>

<h1 align="center">Claude Utility Skills</h1>

<p align="center">
  <strong>A curated collection of specialized skills for Claude Code</strong>
  <br>
  <em>Skill creation, MCP server building, documentation, testing, communications, and research</em>
</p>

<p align="center">
  <a href="#features">Features</a> &middot;
  <a href="#quick-start">Quick Start</a> &middot;
  <a href="#skills-overview">Skills</a> &middot;
  <a href="#project-structure">Structure</a> &middot;
  <a href="#contributing">Contributing</a>
</p>

---

## Features

| Feature | Skill | Description |
|---------|-------|-------------|
| Skill Creation | [skill-creator](skills/skill-creator/SKILL.md) | End-to-end guide for building Claude Code skills, including SKILL.md format, workflows, and best practices |
| MCP Server Building | [mcp-builder](skills/mcp-builder/SKILL.md) | Build MCP servers with FastMCP (Python) or TypeScript SDK, with evaluation scripts and reference docs |
| Anthropic Documentation | [anthropic-docs](skills/anthropic-docs/SKILL.md) | Comprehensive Anthropic knowledge base: API guide, models, Claude Code, research papers, safety policy |
| Web App Testing | [webapp-testing](skills/webapp-testing/SKILL.md) | Playwright-based web app testing with screenshots, browser logs, and UI debugging workflows |
| Internal Communications | [internal-comms](skills/internal-comms/SKILL.md) | Templates for status reports, leadership updates, newsletters, FAQ answers, and incident reports |
| Research Notes | [history-note-processor](skills/history-note-processor/SKILL.md) | Four-step deep reading method with YAML frontmatter and Mermaid diagram generation |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-utility-skills.git
```

### Usage

Skills are automatically available to Claude Code after installation. Use natural language to invoke them:

```text
"Create a new skill"              -> skill-creator
"Build an MCP server"             -> mcp-builder
"Test my web app"                 -> webapp-testing
"Write a status report"           -> internal-comms
"Look up Anthropic API docs"      -> anthropic-docs
"Process these history notes"     -> history-note-processor
```

Or reference a skill directly:

```text
"Use the mcp-builder skill to scaffold a Python MCP server"
```

---

## Skills Overview

### Development Tools

- **[skill-creator](skills/skill-creator/SKILL.md)** -- Complete guide to creating Claude Code skills. Includes `init_skill.py` for scaffolding, `package_skill.py` for packaging, and `quick_validate.py` for validation.
- **[mcp-builder](skills/mcp-builder/SKILL.md)** -- Reference-driven MCP server creation. Ships with Python/Node.js server references, best practices guide, and an evaluation framework.

### Knowledge Base

- **[anthropic-docs](skills/anthropic-docs/SKILL.md)** -- Curated Anthropic documentation covering the API, model selection, Claude Code features, engineering blog highlights, research papers, and safety policy.

### Communications

- **[internal-comms](skills/internal-comms/SKILL.md)** -- Battle-tested templates for company newsletters, 3P updates, FAQ answers, and general communications.

### Testing

- **[webapp-testing](skills/webapp-testing/SKILL.md)** -- Playwright-powered web app testing skill with example scripts for console logging, element discovery, and static HTML automation.

### Research

- **[history-note-processor](skills/history-note-processor/SKILL.md)** -- Deep reading and note-processing workflow with structured templates and API references.

---

## Project Structure

```
claude-utility-skills/
├── LICENSE                          # MIT License
├── README.md                        # This file
├── SKILL.md                         # Root skill index
├── CONTRIBUTING.md                  # Contribution guidelines
├── CHANGELOG.md                     # Release history
├── .github/
│   ├── workflows/
│   │   └── claude-review.yml        # Claude Code review action
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.yml           # Bug report template
│   │   ├── feature_request.yml      # Feature request template
│   │   └── config.yml               # Issue template config
│   └── PULL_REQUEST_TEMPLATE.md     # PR template
└── skills/
    ├── skill-creator/               # Skill creation guide + scripts
    │   ├── SKILL.md
    │   ├── references/
    │   └── scripts/
    ├── mcp-builder/                 # MCP server building guide
    │   ├── SKILL.md
    │   ├── reference/
    │   └── scripts/
    ├── anthropic-docs/              # Anthropic documentation KB
    │   ├── SKILL.md
    │   ├── api-guide.md
    │   ├── claude-code.md
    │   ├── engineering-blog.md
    │   ├── models.md
    │   ├── research-papers.md
    │   └── safety-policy.md
    ├── internal-comms/              # Internal communications
    │   ├── SKILL.md
    │   └── examples/
    ├── webapp-testing/              # Web app testing
    │   ├── SKILL.md
    │   ├── examples/
    │   └── scripts/
    └── history-note-processor/      # Research note processing
        ├── SKILL.md
        └── references/
```

---

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to submit skills, report bugs, and propose features.

---

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

<p align="center">
  <sub>Built with collaboration between human and AI</sub>
</p>
