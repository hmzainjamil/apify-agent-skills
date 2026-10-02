# Apify Agent Skills

A multi-platform instruction pack for working with Apify Actors. It includes Claude Code plugin metadata, a Gemini extension manifest, four skills, one Actor creation command, reference guides, and a script that generates the skills index.

This repository provides instructions and templates. It is not itself a hosted scraper service or a bundled collection of the third-party Actors described in its guides.

## Included

| Path | Purpose |
|---|---|
| `skills/apify-ultimate-scraper/` | Guidance for choosing and running Apify Actors through the Apify CLI |
| `skills/apify-actor-development/` | Actor development and deployment workflow |
| `skills/apify-actorization/` | Guidance for adapting software to the Actor model |
| `skills/apify-generate-output-schema/` | Guidance for deriving Actor schemas from source |
| `commands/create-actor.md` | Guided Actor creation command |
| `agents/AGENTS.md` | Generated skills index for agent hosts |
| `scripts/generate_agents.py` | Generates that index and validates marketplace metadata |
| `.claude-plugin/` | Claude Code plugin and marketplace metadata |
| `gemini-extension.json` | Gemini extension metadata |

Skill-specific reference files describe schemas, Actor patterns, data stores, workflows, and supported Actor examples.

## Requirements

- A compatible AI agent host for Markdown-based skill instructions.
- Apify CLI and an authorized Apify account for workflows that create, run, or deploy Actors.
- `uv` and Python 3.10 or later to run `scripts/generate_agents.py`.

The Claude marketplace metadata names the upstream Apify project and Apache-2.0 license. This repository is a fork or mirror presentation of those materials; check upstream and the license files before redistributing. The local tree has no root LICENSE file.

## Use

Clone and inspect the repository:

```bash
git clone https://github.com/hmzainjamil/apify-agent-skills.git
cd apify-agent-skills
```

Use the skill instructions through your host's documented setup and discovery process. The repository has no installer script. The plugin and extension manifests provide host metadata but do not guarantee that a host version will load them.

To regenerate the agent skills index and validate marketplace consistency:

```bash
uv run scripts/generate_agents.py
```

This writes `agents/AGENTS.md`. Review the diff before committing generated changes.

## External services, data and costs

The scraper guidance can invoke third-party Apify Actors through the Apify CLI. Those runs may send requests to external websites and store results in Apify datasets or key-value stores. Actor availability, permissions, pricing, site rules, and data retention are controlled by Apify, each Actor publisher, and the target service.

- Review the selected Actor's documentation, permissions, pricing, and output before running it.
- Use a scoped `APIFY_TOKEN`; never paste tokens into prompts, command history, committed files, or generated reports.
- Scrape only data and sites you are authorized to access. Follow applicable terms, privacy rules, and data minimization requirements.
- Avoid collecting sensitive personal information unless you have a lawful basis and approved handling.

## Limitations

- Skill files are instructions; tool access and behavior depend on the host.
- Actors named in the guides are external services, not included code in this repository.
- No benchmark, test suite, or cost guarantee is declared here.
- Plugin metadata identifies Apify as author and points to the upstream repository. Verify source attribution and license obligations before repackaging.

## Repository map

- [Skills](skills/apify-ultimate-scraper/SKILL.md)
- [Actor creation command](commands/create-actor.md)
- [Generated skills index](agents/AGENTS.md)
- [Index generator](scripts/generate_agents.py)
- [Claude plugin metadata](.claude-plugin/plugin.json)
- [Gemini extension metadata](gemini-extension.json)

## Contributing

Open an issue with the relevant skill or reference path, expected behavior, and a safe example. Do not include tokens, private account data, or scraped personal information.

## Security and privacy

See [SECURITY.md](SECURITY.md) for token, scraping, and external-service guidance.

## Attribution and license

Plugin metadata points to [Apify's upstream agent-skills repository](https://github.com/apify/agent-skills) and identifies Apache-2.0. This fork's tree does not include a root license file. Verify the upstream license and required notices before redistributing.
