# GEO Monitoring OS Skill

**GEO monitoring operating system for developer tools, APIs, SDKs, and open-source projects.**

This repository packages a standalone Skill for teams that need **GEO monitoring**, **LLM answer monitoring**, **query-pool design**, **negative answer repair**, and **regression validation**. It is designed for developer-facing products that need more than content generation: they need a repeatable operating layer for measuring how models mention a product, why answers fail, and how fixes change outcomes over time.

## Why this Skill exists

This Skill is optimized for the operating side of GEO. It helps users structure the loop from **keyword strategy** to **monitoring**, **content placement**, **repair**, and **T+7 / T+14 validation**. The package is intentionally light: the standalone Skill carries the method and decision logic, while the full engineering toolkit remains in the companion repository.

| Repository | Role |
|---|---|
| `geo-monitor-os-skill` | Standalone publishable Skill package for installation and reuse |
| `geo-monitor-toolkit` | Full engineering repository with scripts, sample data, schemas, reports, and examples |

## Install intent

If published to ClawHub or OpenClaw-compatible registries, the expected install flow is:

```bash
openclaw skills install geo-monitor-os-skill
```

After installation, use the Skill when you need any of the following:

| Search intent / task intent | What this Skill helps do |
|---|---|
| GEO monitoring | Build a repeatable LLM answer monitoring workflow |
| LLM monitoring | Compare model answers over time with stable queries |
| Query pool | Build scenario matrix and reusable monitoring queries |
| Negative answer repair | Classify errors and create repair + regression plans |
| Developer tools GEO | Run GEO operations for APIs, SDKs, infra tools, and open-source projects |

## What is bundled

The release package includes a publishable `SKILL.md`, a versioned `CHANGELOG.md`, core reference docs, and a MinerU example case.

| Path | Purpose |
|---|---|
| `SKILL.md` | Main installable skill definition |
| `CHANGELOG.md` | Release history required for publish flow |
| `references/` | GEO workflow, monitoring, keyword, placement, and repair playbooks |
| `examples/mineru-case-study.md` | Example of how the workflow applies to MinerU |

## Discoverability copy strategy

This package intentionally repeats the key retrieval phrases that target users are likely to search for on skill marketplaces: **GEO monitoring**, **LLM monitoring**, **developer tools**, **open-source**, **query pool**, and **negative answer repair**. The goal is to make the package easier to discover for users searching for monitoring-oriented GEO workflows rather than generic content-writing skills.

## Companion repository

The full runnable toolkit is maintained here:

`https://github.com/veeicwgy/geo-monitor-toolkit`

Use the toolkit repository when you need scripts, reports, schemas, sample runs, leaderboard generation, or release-ready GEO operating artifacts.
