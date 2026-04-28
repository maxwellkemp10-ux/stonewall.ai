---
description: >-
  Stonewall is a legal document intelligence platform for high-volume civil litigation.
  It turns messy case files, email exports, deadlines, and AI review into one governed
  operating surface.
---

# Stonewall

**Legal document intelligence for litigation teams that move fast.**

Stonewall turns scattered emails, pleadings, medical records, deposition material,
spreadsheets, and notes into a searchable, validated, AI-ready litigation corpus.

[![Live Showcase](https://img.shields.io/badge/Live-Showcase-c96b3c?style=for-the-badge)](https://maxwellkemp10-ux.github.io/stonewall-showcase/)
[![Portal Demo](https://img.shields.io/badge/Open-Portal_Demo-111827?style=for-the-badge)](https://maxwellkemp10-ux.github.io/stonewall-showcase/portal/)
[![Official Brief](https://img.shields.io/badge/Read-Official_Brief-f4ede3?style=for-the-badge&labelColor=171310)](https://maxwellkemp10-ux.github.io/stonewall-showcase/official-brief.html)
[![GitBook](https://img.shields.io/badge/GitBook-Product_Book-3884ff?style=for-the-badge)](https://maxwell-kemp.gitbook.io/stonewall-qb3/stonewall-showcase)

---

## The pitch

Law firms do not need another document dump.

They need a command surface that answers:

- What changed?
- What matters now?
- What deadlines are moving?
- Which documents support the next filing, deposition, demand, or client update?
- Which facts are verified, and which still need QC?

Stonewall is that layer.

---

## What it does

| Surface | Outcome |
| --- | ---: |
| **Ingestion** | Pulls OneDrive, Outlook, PDF, DOCX, XLSX, CSV, EML, MSG, TXT, HTML, XML, and ZIP material into a normalized corpus. |
| **Classification** | Extracts dates, parties, claim numbers, document types, matter links, and workflow signals. |
| **Notion Sync** | Turns case data into an operator-facing matter board with dates, status, links, and review queues. |
| **AI Review** | Uses Claude and OpenAI workflows for summarization, classification, recall, and tactical drafting support. |
| **QC Automation** | Runs validation sweeps so bad metadata, missing links, and drift are visible before they become liability. |
| **Publication** | Ships polished static surfaces for demos, briefs, portal views, and stakeholder review. |

---

## Why it wins

- **Built for litigation reality.** Messy exports, late records, fragmented folders, and deadline pressure are first-class design constraints.
- **Operator-first.** The platform is not just storage. It stages the next move.
- **AI with guardrails.** Structured sidecars, source links, validation, and review queues keep outputs traceable.
- **Static where possible. Automated where useful.** Fast to deploy, easy to inspect, hard to break.
- **Commercially legible.** Showcase, portal, official brief, and GitBook all tell one clean product story.

---

## Proof points

| Metric | Scale |
| --- | ---: |
| Artifacts cataloged | 1,200+ |
| Active matters represented | 60+ |
| Behavioral patterns indexed | 197 |
| Emails processed | 6,000+ |
| Artifact classes | 23 |
| Delivery surfaces | GitHub Pages, Portal, GitBook, Official Brief |

---

## Product surfaces

- **[Live showcase](https://maxwellkemp10-ux.github.io/stonewall-showcase/)** — executive overview and product narrative.
- **[Portal demo](https://maxwellkemp10-ux.github.io/stonewall-showcase/portal/)** — dashboard-style operator experience.
- **[Official brief](https://maxwellkemp10-ux.github.io/stonewall-showcase/official-brief.html)** — polished business and architecture brief.
- **[Workflow notes](https://maxwellkemp10-ux.github.io/stonewall-showcase/insights.html)** — implementation and operating model notes.
- **[GitBook edition](https://maxwell-kemp.gitbook.io/stonewall-qb3/stonewall-showcase)** — long-form product book.

---

## Architecture

```text
OneDrive / Outlook / Case Files
            |
            v
      Ingestion Pipeline
            |
            v
  Parsing + Markdown Sidecars
            |
            v
 Classification + AI Review
            |
            v
      Notion Operator Layer
            |
            v
 QC Reports + Static Showcase
```

The system favors inspectable files, repeatable scripts, environment-based configuration,
and CI-visible checks over opaque one-off automation.

---

## Stack

| Layer | Tools |
| --- | --- |
| Runtime | Python 3.11+, Node.js 20+, PowerShell 7+ |
| Package management | `uv`, `npm` |
| AI | Anthropic Claude API, OpenAI API |
| Case management | Notion API |
| Storage | Microsoft OneDrive |
| Automation | GitHub Actions |
| Delivery | GitHub Pages, GitBook, static HTML |

---

## Repository map

```text
stonewall-showcase/
├── docs/                 # GitHub Pages showcase and portal
├── scripts/              # ingestion, sync, QC, and reporting automation
├── agents/               # AI agent configuration
├── tests/                # validation and regression tests
├── .github/workflows/    # CI/CD pipelines
├── .env.example          # required environment variables
├── PRODUCT_ARCHITECTURE.md
├── OFFICIAL_BRIEF.md
└── README.md
```

---

## Security posture

- No hardcoded credentials.
- API tokens and database IDs come from environment variables.
- Public showcase content is sanitized for demo use.
- QC scripts are designed to catch drift before publication.

---

## Bottom line

**Stonewall converts litigation chaos into operational leverage.**

It is the control plane between the document mess and the legal move that wins the day.
