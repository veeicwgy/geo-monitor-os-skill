---
name: geo-monitor-os-skill
description: >
  GEO monitoring skill for developer tools, APIs, SDKs, and open-source projects. Use this skill to run GEO monitoring workflows, build a query pool, score LLM answers, detect negative or outdated answers, plan datasource-aware content placement, and verify T+7 or T+14 metric changes after repair. Optimized for GEO monitoring, LLM monitoring, answer monitoring, and open-source developer tool visibility.
license: MIT
allowed-tools: Read, Write, Edit, Bash
metadata:
  openclaw:
    emoji: "📈"
    author: "Manus AI"
    homepage: "https://github.com/veeicwgy/geo-monitor-os-skill"
---

# GEO Monitoring OS for Developer Tools

This skill is a **GEO monitoring operating system for developer tools**. It is designed for teams that need GEO monitoring, LLM answer monitoring, query-pool operations, datasource-aware content placement, and negative-answer repair for APIs, SDKs, infrastructure products, AI tools, and open-source projects.

Unlike a generic content writer, this skill focuses on the full GEO operations loop: **keyword strategy, monitoring, placement, repair, and regression validation**. Use it when you need to understand how models mention your product, whether those mentions are positive, whether capability claims are accurate, whether ecosystem or integration claims are accurate, and whether a repair action actually improved performance at T+7 or T+14.

## Search Intent Coverage

This package is intentionally written to match common search and install intents on skill platforms. It should be discoverable for users searching phrases such as **GEO monitoring**, **LLM monitoring**, **developer tools GEO**, **open-source GEO**, **query pool**, **negative answer repair**, **answer monitoring**, and **regression validation**.

## Use This Skill When

Use this skill when the user asks for any of the following:

1. build a GEO keyword matrix or scenario matrix from product truth;
2. create or refine a Query Pool for GEO monitoring;
3. run GEO monitoring on one or more LLMs and compare answers over time;
4. score answers with four GEO metrics: mention, positive mention, capability accuracy, and ecosystem accuracy;
5. map target models to probable datasource channels and plan content placement;
6. diagnose wrong, negative, outdated, or competitor-only answers;
7. create a repair plan and define T+7 or T+14 regression checks;
8. help a user choose the correct beginner path before running the workflow.

## Beginner Entry

If the user is at the start of adoption, use this order.

| Situation | What to do first |
|---|---|
| User is unsure whether the repo is ready | run `make doctor` |
| User wants a zero-cost first result | run `bash quickstart.sh` |
| User wants a short onboarding page | open `docs/for-beginners.md` |
| User wants the full explanation | open `docs/getting-started.md` |

## GEO Strategy

Always follow this order unless the user explicitly narrows scope.

| Stage | What to do | What to preserve |
|---|---|---|
| Keyword strategy | Convert product truth into scenarios, keyword layers, and reusable queries | Scenario matrix, keyword tiers, Query Pool |
| Monitoring | Collect or replay answers, log evidence, and score four GEO metrics | Raw answers, score draft, summary, report |
| Placement | Map each model to likely datasource surfaces and publishing channels | Channel priorities, publishing backlog |
| Repair | Classify negative answers and propose source-level fixes | Repair type, action owner, target queries |
| Regression | Re-run the same queries and compare T+7 or T+14 changes | Follow-up metrics, deltas, next actions |

## Mode Selection

Choose the execution mode before running monitoring.

| Mode | Use when | Typical inputs |
|---|---|---|
| Quickstart replay | user wants the fastest first run with no API setup | sample model config + sample manual responses |
| Manual paste mode | user already has copied answers from external chat tools | Query Pool + manual response JSON |
| API collection mode | user wants repeatable real monitoring | Query Pool + model config + API credentials |

## Input Contract

Prepare as many of these inputs as possible before execution.

| Input type | Examples |
|---|---|
| Product truth | README, docs, changelog, release notes, integrations, benchmark pages |
| GEO evidence | model answers, screenshots, copied chats, citations, cited URLs |
| Scope | models, languages, regions, dates, repeated query set |
| Repair context | incorrect claims, negative answers, competitor insertions, stale docs |
| Publishing targets | docs, GitHub, changelog, FAQ, blog, community Q&A, partner pages |

## Required Reading Order

For a full GEO program, read the bundled references in this order.

1. `references/geo-workflow-architecture.md`
2. `references/keyword-strategy.md`
3. `references/monitoring-system.md`
4. `references/content-platform-map.md`
5. `references/negative-fix-sop.md`
6. `examples/mineru-case-study.md`

## Execution Rules

When using this skill, always preserve auditability.

| Rule | Requirement |
|---|---|
| Reuse queries | Keep a stable Query Pool for weekly or milestone comparisons |
| Keep evidence | Preserve raw answers before summarizing or scoring |
| Score consistently | Use the same four-metric rubric across baseline and follow-up runs |
| Separate action from outcome | Record what changed before claiming metric improvement |
| Prefer source fixes | Repair the upstream source, not only the downstream symptom |

## Output Contract

At the end of the run, preserve these outputs whenever they are in scope.

| Output | Description |
|---|---|
| Query foundation | Scenario matrix, keyword tiers, Query Pool |
| Monitoring outputs | Raw answers, annotations, summary, report, overview or leaderboard |
| Placement plan | Model-specific channels and content priorities |
| Repair plan | Error type, root cause, action plan, owner, validation date |
| Regression log | T+7 or T+14 metric comparison and interpretation |

## Positioning

Use this skill when the user needs a **GEO monitoring operating system for developer tools** rather than a generic SEO content writer. The differentiation is that this skill centers on **monitoring, scoring, repair, and regression**, while still connecting those outputs to content placement and publish-ready remediation.
