# [stnwl.ai](https://www.stnwl.ai/)
# Stonewall — Legal Intelligence Platform

[![Stonewall Home](https://img.shields.io/badge/Home-stonewall.esq-c96b3c?style=for-the-badge)](https://stonewall.esq/)
[![Showcase Pages](https://img.shields.io/badge/Showcase-GitHub_Pages-111827?style=for-the-badge)](https://maxwellkemp10-ux.github.io/stonewall-showcase/)
[![Official Brief](https://img.shields.io/badge/Read-Official_Brief-1d1d1d?style=for-the-badge)](https://maxwellkemp10-ux.github.io/stonewall-showcase/official-brief.html)
[![Portal Demo](https://img.shields.io/badge/Open-Portal_Demo-0b57d0?style=for-the-badge)](https://maxwellkemp10-ux.github.io/stonewall-showcase/portal/)
[![Python](https://img.shields.io/badge/Python-3.11%2B-3776ab?style=flat-square)](#tech-stack)
[![Node](https://img.shields.io/badge/Node.js-20%2B-5fa04e?style=flat-square)](#tech-stack)
[![Notion API](https://img.shields.io/badge/Notion-API-000000?style=flat-square)](#innovation-stack)
[![Claude](https://img.shields.io/badge/Claude-Workflow_Intelligence-d97757?style=flat-square)](#innovation-stack)
[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-QC_Automation-2088ff?style=flat-square)](#verification-and-qc)

> Stonewall turns litigation exhaust into a live operating corpus. OneDrive folders, Outlook exports, Notion matters, repo-side validation, and AI-assisted classification all move through one system so a legal team can search, cross-check, brief, and act without losing the thread.

Stonewall is a production-grade legal document intelligence platform built for high-volume civil litigation. It is a workflow engine for turning emails, filings, deposition material, medical records, and case events into a searchable, auditable operating surface.

The repository shows the product logic, the automation architecture, and the delivery surfaces that make the system commercially viable: a litigation corpus, a Notion operator layer, validation-first automation, tactical briefing workflows, and a static portal that can be deployed instantly.

## Live Surfaces

- [Stonewall home](https://stonewall.esq/) — the canonical product narrative.
- [Showcase Pages](https://maxwellkemp10-ux.github.io/stonewall-showcase/) — the fastest way to understand this repository exhibit.
- [Official brief](https://maxwellkemp10-ux.github.io/stonewall-showcase/official-brief.html) — the boardroom-safe narrative version.
- [Portal demo](https://maxwellkemp10-ux.github.io/stonewall-showcase/portal/) — the operator-facing command surface.
- [Architecture note](https://github.com/maxwellkemp10-ux/stonewall-showcase/blob/main/docs/ARCHITECTURE.md) — layer-by-layer technical walkthrough.

## By The Numbers

| Metric | Scale |
| --- | ---: |
| Artifacts cataloged | 1,200+ |
| Active cases represented | 60+ |
| Behavioral patterns indexed | 197 |
| Characters profiled | 120+ |
| Emails processed | 6,000+ |
| Artifact types classified | 23 |

## Why This Platform Hits

- **Notion as the live operator layer.** Matters, dates, holds, and cross-links stay visible to the humans actually running the docket.
- **Workflow-ready, not archive-only.** The same corpus that supports search and reporting also sharpens deposition prep, deadline control, and downstream demand packet readiness.
- **Verification built in.** QC scripts and GitHub Actions keep the front door honest instead of letting bad metadata pile up.
- **DataGavel workflow readiness.** The factual substrate is organized before the packet, report, or damages workflow begins.
- **Live deposition tailoring.** New filings, transcript derivatives, chronology, and actor-level context can feed outline changes in real time.

## Innovation Stack

### 1. Litigation Corpus

Stonewall treats the corpus as a governed operating layer instead of burying knowledge inside a database no one can inspect.

### 2. Notion Operator Layer

`notion_wire_cases.py`, `notion_case_dates.py`, `notion_consolidate_emails.py`, and the repair scripts turn Notion into an execution surface rather than a passive notes app.

### 3. Verification-First Automation

`qc_sweep.mjs`, `repo_sweep.py`, `verify_repo_consistency.py`, and `tactical_brief.py` create a loop where ingestion, sync, and audit are part of one operating rhythm.

### 4. Static Publication Surfaces

The platform can be shown cleanly through GitHub Pages and a static portal because the architecture underneath is real.

## Architecture

```text
OneDrive / Outlook Export
          |
          v
    Ingestion Layer
          |
          v
   Processing Layer
          |
          v
    Notion Sync Layer
          |
          v
   AI Tagging Layer
          |
          v
 Verification + Reporting
          |
          v
   Portal / Brief
```

## Representative Commands

```bash
python scripts/tactical_brief.py today
uv run python scripts/notion_case_dates.py --csv case_dates.csv
NOTION_TOKEN=ntn_xxx node scripts/qc_sweep.mjs
python scripts/verify_repo_consistency.py
```

## Tech Stack

| Layer | Technology |
| --- | --- |
| Languages | Python 3.11+, Node.js 20+, PowerShell 7+ |
| AI | Anthropic Claude API, OpenAI API |
| Knowledge layer | Notion API |
| Source reservoir | Microsoft OneDrive |
| CI / automation | GitHub Actions |
| Delivery surfaces | GitHub Pages, static portal |

The public repository is the proof surface. The implementation work is the product.


inquiries@stnwl.ai

2026 — Stonewall Legal Enterprises
