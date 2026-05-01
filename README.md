# Stonewall

**Legal document intelligence for litigation teams that move fast.**

Stonewall turns scattered emails, pleadings, medical records, deposition material,
spreadsheets, and notes into a searchable, validated, AI-ready litigation corpus.

[![Stonewall Home](https://img.shields.io/badge/Home-stonewall.esq-c96b3c?style=for-the-badge)](https://stonewall.esq/)
[![Showcase Pages](https://img.shields.io/badge/Showcase-GitHub_Pages-111827?style=for-the-badge)](https://maxwellkemp10-ux.github.io/stonewall-showcase/)
[![Operator App](https://img.shields.io/badge/App-app.stonewall.esq-f4ede3?style=for-the-badge&labelColor=171310)](https://app.stonewall.esq/)

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
- **Commercially legible.** Showcase, portal, and official brief all tell one clean product story.

---

## Proof points

| Metric | Scale |
| --- | ---: |
| Artifacts cataloged | 1,200+ |
| Active matters represented | 60+ |
| Behavioral patterns indexed | 197 |
| Emails processed | 6,000+ |
| Artifact classes | 23 |
| Delivery surfaces | GitHub Pages, Portal, Official Brief |

---

## Product surfaces

- **[Stonewall home](https://stonewall.esq/)** — canonical public product narrative.
- **[Showcase Pages](https://maxwellkemp10-ux.github.io/stonewall-showcase/)** — public engineering exhibit for this repository.
- **[Operator app](https://app.stonewall.esq/)** — authenticated command cockpit.
- **[Graph demo](https://stonewall.esq/portal/#graph)** — aggregate visual proof on the public front door.

`stonewall.esq` is owned by the canonical Stonewall publishing stack. This
showcase repository publishes through GitHub Pages without a custom apex claim.

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
| Delivery | GitHub Pages, static HTML |

---

## Repository map

```text
stonewall-showcase/
├── docs/                 # GitHub Pages showcase and portal
│   ├── overview/         # product docs (official brief, architecture, workflow surfaces)
│   ├── showcase/         # showcase narrative and synergy docs
│   └── portal/           # operator portal app and data snapshots
├── scripts/              # ingestion, sync, QC, and reporting automation
├── agents/               # AI agent configuration
├── tests/                # validation and regression tests
├── archive/              # archived publication-runbook reference material
├── sample-corpus/        # neutral sample reference material for demos
├── .github/workflows/    # CI/CD pipelines
├── .env.example          # required environment variables
└── README.md
```

---

## Security posture

- No hardcoded credentials.
- API tokens and database IDs come from environment variables.
- Public showcase content uses neutral sample labels for demo use.
- QC scripts are designed to catch drift before publication.

---

## Bottom line

**Stonewall converts litigation chaos into operational leverage.**

It is the control plane between the document mess and the legal move that wins the day.
