# Contributing

Thank you for improving the GEO Monitoring OS Skill.

This repository is the **standalone publishable Skill package**. Keep it focused on installable skill content and platform-facing discoverability. Do not copy the whole engineering toolkit into this repository unless the publish format requires it.

## Contribution scope

Good contributions include improving GEO monitoring instructions, refining search-facing copy, tightening the input/output contract, updating bundled references, and advancing release packaging quality.

| Area | Expected standard |
|---|---|
| `SKILL.md` | Keep the first section highly descriptive for GEO monitoring, LLM monitoring, developer tools, open-source, query pool, and negative answer repair |
| `CHANGELOG.md` | Bump semver and record user-visible changes before publish |
| `README.md` | Keep install intent, positioning, and companion repository relationship clear |
| `references/` | Update only stable methodology documents that strengthen the skill |

## Release checklist

Before publishing, complete the following sequence.

| Step | Requirement |
|---|---|
| 1 | Update `SKILL.md` version using semver |
| 2 | Add the new release entry to `CHANGELOG.md` |
| 3 | Re-check that the opening description still targets GEO monitoring search intent |
| 4 | Validate the skill structure locally |
| 5 | Run `clawhub publish` from the skill root when the package is ready |

## Writing rule

Favor concise, search-intent-rich language over verbose narrative. The goal is to help both human users and platform indexing systems understand that this package is a **GEO monitoring operating system for developer tools**.
