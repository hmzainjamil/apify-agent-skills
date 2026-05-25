# apify-agent-skills

> **Apify agent skills — Claude Code skills for web scraping via Apify actors**

![Status](https://img.shields.io/badge/status-active-brightgreen?style=flat)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat)
![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-FF6B35?style=flat)
![Stars](https://img.shields.io/github/stars/hmzainjamil/apify-agent-skills?style=flat)
![Last Commit](https://img.shields.io/github/last-commit/hmzainjamil/apify-agent-skills?style=flat)

---

## CONCEPTS

| Concept | Description |
|---|---|
| **Apify** | Core apify capability for apify-agent-skills workflows |
| **Agent** | Core agent capability for apify-agent-skills workflows |
| **Scraping** | Core scraping capability for apify-agent-skills workflows |
| **Extraction** | Core extraction capability for apify-agent-skills workflows |
| **Actor** | Core actor capability for apify-agent-skills workflows |
| **Data** | Core data capability for apify-agent-skills workflows |
| **Claude** | Core claude capability for apify-agent-skills workflows |
| **Automation** | Core automation capability for apify-agent-skills workflows |

---

## 🔥 Hot Commands

```bash
# Activate skill
claude --skill apify-agent-skills 'your task'

# Quick workflow
claude 'apify automation task'

# Get capabilities
claude 'what can apify-agent-skills do?'
```

## ■ tip
> Mention **apify** or **agent** in your prompt to auto-activate this skill.

---

## ☠️ STARTUPS / BUSINESSES

- **Agencies**: automate apify workflows for clients at scale
- **Founders**: ship agent features 10x faster with Claude
- **Freelancers**: deliver scraping work with AI-assisted precision

---

## Features

- Apify automation and orchestration
- Agent automation and orchestration
- Scraping automation and orchestration
- Extraction automation and orchestration
- Actor automation and orchestration
- Data automation and orchestration

---

## Installation

```bash
git clone https://github.com/hmzainjamil/apify-agent-skills.git
cd apify-agent-skills
```

---

## Usage

```bash
# In Claude Code
/apify-agent-skills
claude 'apify task here'
```

---

## Configuration

| Variable | Description | Default |
|---|---|---|
| `API_KEY` | Primary API key for service access | Required |
| `MODEL` | AI model to use | claude-3-5-sonnet |
| `DEBUG` | Enable verbose debug output | false |
| `MAX_TOKENS` | Max token budget per request | 8192 |
| `TIMEOUT` | Request timeout in seconds | 30 |
| `LOG_LEVEL` | Logging verbosity | info |

---

## Architecture

```
apify-agent-skills/
├── README.md           # This file
├── SKILL.md            # Claude Code skill definition
├── scripts/            # Automation and utility scripts
├── templates/          # Output and prompt templates
├── examples/           # Usage examples and demos
├── tests/              # Unit and integration tests
└── docs/               # Extended documentation
    ├── setup.md        # Setup guide
    ├── api.md          # API reference
    └── faq.md          # Frequently asked questions
```

---

## Examples

### Basic Usage

```bash
# Activate in Claude Code
claude --skill apify-agent-skills "your task here"

# With options
claude --skill apify-agent-skills --verbose "detailed task"
```

### Advanced Workflow

```bash
# Chain with other skills
claude --skill apify-agent-skills "step 1" | claude --skill summarize

# Batch processing
for item in list; do
  claude --skill apify-agent-skills "process $item"
done
```

---

## Troubleshooting

| Issue | Cause | Fix |
|---|---|---|
| Auth fails | Invalid/expired API key | Re-export key in shell profile |
| Timeout error | Network latency or large payload | Increase TIMEOUT value |
| Empty output | Prompt too vague | Add more context to request |
| Rate limit hit | Too many requests | Add delay between calls |
| Model error | Unsupported model version | Update MODEL variable |
| Import error | Missing dependency | Run pip install -r requirements.txt |

---

## Comparison

| Feature | This Skill | Alternative A | Alternative B |
|---|---|---|---|
| Claude Code native | ✅ | ❌ | ✅ |
| Auto-activation | ✅ | ✅ | ❌ |
| Free to use | ✅ | ❌ | ✅ |
| Production ready | ✅ | ✅ | ❌ |
| Active maintenance | ✅ | ❌ | ❌ |

---

## Contributing

1. Fork this repo
2. Create feature branch: `git checkout -b feat/your-feature`
3. Commit changes: `git commit -m 'feat: add feature'`
4. Push: `git push origin feat/your-feature`
5. Open PR

---

## Changelog

| Version | Changes |
|---|---|
| v2.0 | Major refactor, Claude 4 support |
| v1.5 | Added auto-activation keywords |
| v1.0 | Initial release |

---

## ⭐ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=hmzainjamil/apify-agent-skills&type=Date)](https://star-history.com/#hmzainjamil/apify-agent-skills&Date)

---

## 📜 License

MIT — free to use, modify, and distribute.

---

Made with ❤️ by [@hmzainjamil](https://github.com/hmzainjamil)
