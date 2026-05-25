# apify-agent-skills

> **Apify agent skills for Claude Code — web scraping and data extraction via Apify actors**

![Status](https://img.shields.io/badge/status-active-brightgreen?style=flat)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat)
![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-FF6B35?style=flat)
![Stars](https://img.shields.io/github/stars/hmzainjamil/apify-agent-skills?style=flat)
![Last Commit](https://img.shields.io/github/last-commit/hmzainjamil/apify-agent-skills?style=flat)

---

## CONCEPTS

| Concept | Description |
|---|---|
| **Actor** | Serverless scraping unit on Apify platform |
| **Dataset** | Structured output storage for scraped data |
| **Proxy** | Rotating residential proxies to avoid blocks |
| **Scheduler** | Cron-based actor execution |
| **Webhook** | Event trigger on actor completion |
| **Key-Value Store** | Blob storage for unstructured files |
| **Playwright** | Headless Chrome for dynamic sites |
| **Cheerio** | Fast HTML parser for static sites |

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
- **Founders**: ship agent features 10x faster
- **Freelancers**: deliver scraping work with AI precision

---

## Features

- Apify automation
- Agent automation
- Scraping automation
- Extraction automation
- Actor automation
- Data automation

---

## Installation

```bash
git clone https://github.com/hmzainjamil/apify-agent-skills.git
cd apify-agent-skills
```

---

## Usage

```bash
# Activate skill in Claude Code
claude --skill apify-agent-skills "your task here"

# Quick workflow
claude "apify automation task"

# Get help
claude "what can apify-agent-skills do?"
```

---

## Configuration

| Variable | Description | Default |
|---|---|---|
| `API_KEY` | Primary API key | Required |
| `MODEL` | AI model to use | claude-3-5-sonnet |
| `DEBUG` | Enable verbose debug | false |
| `MAX_TOKENS` | Max token budget | 8192 |
| `TIMEOUT` | Request timeout (sec) | 30 |
| `LOG_LEVEL` | Logging verbosity | info |

---

## Architecture

```
apify-agent-skills/
├── README.md           # Documentation
├── SKILL.md            # Claude Code skill definition
├── scripts/            # Automation scripts
├── templates/          # Output templates
├── examples/           # Usage examples
└── docs/               # Extended documentation
```

---

## Examples

### Basic

```bash
# Simple task
claude --skill apify-agent-skills "apify task"

# Verbose
claude --skill apify-agent-skills --verbose "detailed agent task"
```

### Advanced Pipeline

```bash
# Chain skills
claude --skill apify-agent-skills "step 1" | claude --skill summarize

# Batch run
for item in $(cat list.txt); do
  claude --skill apify-agent-skills "process $item"
done
```

---

## Troubleshooting

| Issue | Cause | Fix |
|---|---|---|
| Auth fails | Invalid API key | Re-export key in shell profile |
| Timeout | Network or large payload | Increase TIMEOUT value |
| Empty output | Prompt too vague | Add more context |
| Rate limit | Too many requests | Add delay between calls |
| Model error | Unsupported version | Update MODEL variable |
| Import error | Missing dependency | Run pip install -r requirements.txt |

---

## Comparison

| Feature | This Skill | Alt A | Alt B |
|---|---|---|---|
| Claude Code native | ✅ | ❌ | ✅ |
| Auto-activation | ✅ | ✅ | ❌ |
| Free to use | ✅ | ❌ | ✅ |
| Production ready | ✅ | ✅ | ❌ |
| Active maintenance | ✅ | ❌ | ❌ |

---

## Changelog

| Version | Changes |
|---|---|
| v2.0 | Claude 4 support, auto-activation |
| v1.5 | Added keyword triggers |
| v1.0 | Initial release |

---

## Contributing

1. Fork → feature branch → commit → PR
2. Follow conventional commits: `feat:`, `fix:`, `docs:`
3. Add tests for new features

---

## ⭐ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=hmzainjamil/apify-agent-skills&type=Date)](https://star-history.com/#hmzainjamil/apify-agent-skills&Date)

---

## 📜 License

MIT — free to use, modify, distribute.

---

Made with ❤️ by [@hmzainjamil](https://github.com/hmzainjamil)
