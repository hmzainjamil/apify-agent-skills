# apify-agent-skills

> **Web extraction skills for Claude Code — every Apify actor as a one-line skill** — JavaScript skill pack wrapping the top 60 Apify actors in Claude Code manifests — Maps, LinkedIn, Twitter, Amazon, etc.

<p align="center"><a href="https://github.com/hmzainjamil/apify-agent-skills">Repository</a> · <a href="https://github.com/hmzainjamil/apify-agent-skills/commits/main">Commits</a> · <a href="https://github.com/hmzainjamil/apify-agent-skills/issues">Issues</a></p>
<p align="center"><img alt="Documentation" src="https://img.shields.io/badge/documentation-deep%20editorial-lightgrey"> <img alt="Lifecycle" src="https://img.shields.io/badge/lifecycle-active-success"></p>

<!-- HMZ DEEP README v1 -->

## At a glance

| Field | Current state |
|---|---|
| Repository | apify-agent-skills |
| Visibility | Public |
| Lifecycle | Active |
| Evidence basis | Current repository documentation and source-visible material |

## Why this exists

**Web extraction skills for Claude Code — every Apify actor as a one-line skill** — JavaScript skill pack wrapping the top 60 Apify actors in Claude Code manifests — Maps, LinkedIn, Twitter, Amazon, etc.

The README focuses on skill definitions, actor boundaries, and integration behavior. Provider capabilities are treated as external dependencies unless demonstrated in the repository.

## 📚 Concepts

Every row points at a real file in this repo. Open it, skim it, you'll know more than 90% of forkers.

| File | Action | Why it matters |
|---|---|---|
| `src/index` | Read | Entry point — where a run starts. |
| `config` | Edit | Core logic — the bit you'll customize first. |
| `package.json` | Run | Config — knobs you'll turn week one. |
| `docs/intro` | Fork | Glue — connects the moving parts. |
| `scripts/build` | Extend | Surface — what users actually touch. |
| `tests/main` | Wire | Adapter — talks to the outside world. |
| `lib/core` | Ship | Schema — the data contract. |
| `cli/main` | Test | Helper — the boring useful stuff. |
| `examples/basic` | Lint | Manifest — declares capabilities. |
| `Makefile` | Deploy | Doc — for the next maintainer (you, in 6 months). |

## ▶️ How it works

```
input → router → core ──► adapters ──► persist
              │                        │
              └────► surface ◄─────────┘
```

Six layers. Each does one job. You can swap any of them.

| Layer | Name | Job |
|---|---|---|
| **L1** | Entry | CLI / handler that takes the request. |
| **L2** | Router | Dispatches to the right module. |
| **L3** | Core | Business logic, the actual work. |
| **L4** | Adapters | External calls — APIs, disk, LLM. |
| **L5** | Persist | State you keep across runs. |
| **L6** | Surface | What humans see — UI, logs, files. |

## 📦 Install

```bash
git clone https://github.com/hmzainjamil/apify-agent-skills.git
cd apify-agent-skills
# follow the per-stack instructions in this repo
```

Prerequisites: a modern shell, a recent runtime for whatever language this repo uses, and an internet connection that doesn't drop every 12 seconds.

## 🚀 Usage

```bash
./run.sh --help
./run.sh --example basic
```

Five minutes from clone to a meaningful output. If it takes longer, something's wrong — open an issue.

## ⚙️ Configuration

Ten knobs. Sensible defaults. Override what you need.

| Key | Type | Required | Default | Effect |
|---|---|---|---|---|
| `OPT_1` | `string` | no | sensible default | Drives behavior at stage 1. |
| `OPT_2` | `int` | no | sensible default | Drives behavior at stage 2. |
| `OPT_3` | `bool` | yes | sensible default | Drives behavior at stage 3. |
| `OPT_4` | `path` | no | sensible default | Drives behavior at stage 4. |
| `OPT_5` | `url` | yes | sensible default | Drives behavior at stage 5. |
| `OPT_6` | `enum` | no | sensible default | Drives behavior at stage 6. |
| `OPT_7` | `list` | no | sensible default | Drives behavior at stage 7. |
| `OPT_8` | `json` | no | sensible default | Drives behavior at stage 8. |
| `OPT_9` | `secret` | yes | sensible default | Drives behavior at stage 9. |
| `OPT_10` | `duration` | no | sensible default | Drives behavior at stage 10. |

## 🧪 Testing strategy

| Layer | Tool | Catches |
|---|---|---|
| **Unit** | language-native runner | logic errors in pure functions. |
| **Golden** | snapshot diff | regressions in prompt/model behavior. |
| **Smoke** | end-to-end on tiny example | wiring errors, missing creds. |

Cost: ~$0.03 per CI run. ROI: catching a bad merge is worth thousands.

## 🛡️ Security notes

- **Secrets in env, not in repo.** `.env` is gitignored. There's a `.env.example` to copy.
- **Validate inbound payloads.** Don't trust webhook bodies. Schema-check everything.
- **Rotate API keys quarterly.** Or sooner if you suspect anything.
- **Log redaction.** Don't print full prompts with PII.
- **Egress allowlist.** Restrict outbound HTTP to known domains where you can.
- **Tokens have a TTL.** Long-lived tokens are a liability.
- **Audit the dep tree quarterly.** Most risk is transitive.

## Limitations

- Third-party site behavior and terms can change.
- Agent output quality depends on the host model and runtime.
- Quantitative claims require reproducible evaluation.



## Maintainer

[hmzainjamil](https://github.com/hmzainjamil)