<div align="center" markdown="1">

# Work Wins & Case Studies

**Analytics · Automation · Operational Reporting · Data Storytelling**

<a href="./"><img src="https://img.shields.io/badge/←_Back_to_Portfolio-1B365D?style=for-the-badge" alt="Back to portfolio"></a>
<a href="./About.html"><img src="https://img.shields.io/badge/About_Me-1B365D?style=for-the-badge" alt="About"></a>
<a href="Daniel_Patterson_Resume.pdf"><img src="https://img.shields.io/badge/Resume-C9A227?style=for-the-badge&logo=readthedocs&logoColor=white" alt="Resume"></a>

<sub>Updated August 2026 · Figures are stated as scale and ratio rather than exact internal amounts</sub>

</div>

<br>

---

## Overview

Over the last two years I have built analytics, automation, and reporting systems that made financial data more accurate, got insights to leadership faster, and gave operations tighter control across cash reconciliation, credit balance, Medicaid AR, bad debt, and refund reconciliation.

In 2026 I was promoted to Business Process Analyst III and given near-full ownership of enterprise-wide bad debt and underperformer reporting across every facility in the network. The flagship bad debt report was selected for presentation up the leadership chain.

| Theme | What it looks like |
|:---|:---|
| **Reconciliation at scale** | Multi-source matching across roughly a billion dollars in annual deposit volume at a 98.5% match rate |
| **Automation** | Manual recurring reports converted into scheduled pipelines with one-click refresh and automated distribution |
| **Payment integrity** | Duplicate detection and root cause analysis driving a sustained ~60% month-over-month reduction |
| **Enterprise reporting** | Frameworks scaled from single-facility pilots to network-wide across 170+ hospitals |
| **Standards** | Report layout standard and audit guidelines adopted across the analyst team |

---

## Flagship: Medicare Cash Reconciliation Platform

**The problem.** The Cash team had no reliable ongoing way to confirm that received cash was being posted timely and accurately. What existed was a manual comparison between two systems.

**What I built.** A reconciliation framework spanning five separate data sources. A large share of the effort went into standardizing account numbers and payment identifiers across systems that each formatted them differently, stripping prefixes, letters, and inconsistent formatting so records could be matched with confidence. On top of the standardized identifiers I built a confidence-scoring model that rates each payment match by how many independent sources support it.

Initial reconciliation covered roughly 37,000 payment records tied to over 29,000 accounts, with about two-thirds independently supported by at least one outside source. From there it evolved into an operational dashboard tracking deposits by facility and fiscal intermediary, calculating true posting lag, the actual number of days between a deposit landing and the matching payment posting, rather than relying on a date-tolerance approximation.

| Measure | Result |
|:---|:---|
| Match rate, deposits traced to posting activity | **98.5%** |
| Match rate by dollar value | **99.5%** |
| Exact penny-level agreements between systems | **5,400+** |
| Median posting lag | **Same day** |
| Unmatched deposits narrowed to actionable exceptions | **113** |

> **Why the median mattered as much as the exceptions.** The reconciliation was commissioned to find problems, and it did surface an auto-posting break worth reviewing. But the same-day median also confirmed that existing posting processes were working well, which is a finding leadership needed just as much and would not have had otherwise.

Full end-to-end build: requirements discovery, identifier standardization, matching and confidence-scoring methodology, and the transition from a one-time workbook analysis into a recurring operational monitoring tool.

---

## Flagship: Enterprise Bad Debt Reporting Program

**The goal.** Give hospital leadership a clean, repeatable read on bad debt: how it trends quarter over quarter, where the biggest cleanup opportunities sit, and which segments drive the picture.

It started as a single-facility pilot, with the structure and visual language designed from the outset to translate to every other facility. The pilot proved out well enough that I was given near-full ownership of the program, and the finished report was selected for presentation up the leadership chain.

The pilot became the flagship implementation for a broader initiative, expanding into an executive package consolidating write-off trends, root-cause classification, financial risk concentration, and improvement recommendations. That analysis surfaced a coordination-of-benefits write-off pattern that led to discussions on new front-end tracking methods.

Rather than looping the per-facility build, I re-architected the reporting logic into a single package covering every facility across the network at once, delivered ahead of a hard deadline and confirmed by the requesting stakeholder same-day. The framework was later extended into a seven-page regional roll-up for Regional Controllers.

---

## Flagship: Credit Balance Operational Report

Built to give the department a single honest picture of credit balance activity: monthly and weekly trends, decentralized versus centralized comparisons, team throughput, payer drivers, and compliance timing.

The design choices carry the report. Daily-average inventory and dollars smooth out noise so trends stay readable. Team drilldowns let managers see accounts, dollars, payer mix, and throughput at their own level. A pre and post view brackets a major operational restructuring, a weekly lens catches inflow shifts and timing outliers, and responsible-party insights show when a payer is driving the numbers.

It became the department-wide standard layout and introduced the Executive Summary plus KPI Box format now used across other departmental reports.

---

## Payment Integrity

<details markdown="1">
<summary><b>Duplicate payment review and monitoring platform</b></summary>

<br>

**The review.** Find the duplicates, determine the cause, quantify exposure, drive remediation. The analysis surfaced seven figures in duplicate payments, roughly 60% from delayed insurance postings, 28% from automatic-posting errors, and 12% from cash-posting errors.

**The fixes.** Improved EDI response tracking, extended the posting-delay threshold to cut false-duplicate flags, tightened detection logic, and added QA checks around large batches. Result was a **~60% month-over-month reduction** with a clean downward trend after remediation, and a segment-level breakdown the team used to build targeted training.

**The platform it became.** I centralized all reporting logic and historical data into a single database-backed source of truth, expanding visibility beyond duplicates to all reviewed postings, small-balance reviews, and team-level workload metrics. Added weekly and monthly trend views, historical tracking, and a calendar heat map so leadership can spot which dates cluster the most duplicate volume. I also built a management review tab for filtering and investigating duplicate populations directly, a gap I identified and closed proactively rather than one that was requested.

I presented the findings to a cross-functional audience of 100+ team members covering financial exposure, root causes, dashboards, and process changes. The work was later featured in an internal recognition program highlighting analyst contributions.

</details>

<details markdown="1">
<summary><b>Due Diligence initiative and automation</b></summary>

<br>

This one was not assigned. I noticed a recurring pattern of stalled, unresolved balances sitting on the active worklist during day-to-day operational work, and built a review process to work through them systematically.

The process included a repeatable review flow to flag and resolve aged worklist balances, a documented process map, and an automated reporting solution. Filters and payer-classification logic went through several rounds of stakeholder feedback before landing.

It recovered a substantial balance population, moved to daily automated distribution with zero calculation errors during team review, and was adopted as an ongoing operational process rather than a one-off.

The framework carried forward. In 2026 I built automated Medicaid, BCBS, and QMB due diligence reports on top of it, together supporting seven figures in substantiated write-offs. Since launch the reports have picked up mass-upload capability, upgraded visuals, and automated exception handling, and moved to a sustainable weekly distribution cadence.

</details>

<details markdown="1">
<summary><b>Automated refund accuracy reconciliation</b></summary>

<br>

Refunds were occasionally being mailed to outdated vendor addresses because manual matching could not keep pace with vendor-file changes.

I built cross-team reconciliation logic matching refund recipients against the current vendor list of record, first using address matching, then re-engineered around a more reliable ID-based match that improved accuracy and cut manual review. The whole thing runs on automated daily distribution to AR teams. No manual pull, no manual review handoff, and the misdirected-refund risk went with it.

</details>

---

## Reporting Frameworks

<details markdown="1">
<summary><b>Underperformers reporting suite</b></summary>

<br>

Leadership needed to see where operational performance was drifting early enough to act. I built the executive summary page for an all-facility underperformers report, consolidating KPIs, root-cause analysis, and facility trends with automated data refresh. After validation work resolved early reporting discrepancies, the report was delivered and went through several enhancement rounds covering calculation methodology and alignment with reporting standards before finalization.

In parallel I built the team-level version: foundational report structure, KPI scorecards, a Cash-to-Net-by-facility view, an out-of-compliance tracker, and a responsible-party analysis page. I then took ownership of scaling that structure across every team through an automated looping process.

</details>

<details markdown="1">
<summary><b>Automated credit balance reporting suite</b></summary>

<br>

A fully automated R and HTML reporting pipeline consolidating operational credit-balance metrics: balance-tier breakdowns, facility-level analytics, responsible-party insights, team workflows covering accounts, compliance, and aging, and aging buckets tied to operational status.

One-click refresh, lower error risk, faster cadence, and a reusable framework I have built other reports on top of since.

</details>

<details markdown="1">
<summary><b>Medicaid AR analysis</b></summary>

<br>

Built to find where balance concentration, plan-level delays, and operational risk were actually sitting.

Findings: balances concentrated in a small number of high-volume facility groups; a handful of payer plan codes accounting for a disproportionate share of impact; select segments seeing discharge-to-payment delays of 400 to 580+ days; and payments concentrated within a specific high-volume claim series.

The report gave the team targeted follow-up insights, clear segmentation to guide operations, auto-refresh capability, and plan-level payment behavior visibility that did not exist before.

</details>

<details markdown="1">
<summary><b>Document processing audit and cleanup</b></summary>

<br>

Built and led an audit and tracking framework supporting a full cleanup of a document-processing backlog, standardizing the review process, flagging processing errors, and capturing accounts needing further research or training. The tooling gave leadership visibility into team-wide progress and supported onboarding as more team members joined the effort.

The initiative closed out a major document category entirely and drove the overall backlog down to roughly **15% of its original size**. I also built reporting to identify documents that failed to post due to missing or incomplete information, enabling targeted root-cause follow-up rather than blanket rework.

</details>

<details markdown="1">
<summary><b>Additional reports and leadership briefings</b></summary>

<br>

- **Medicaid performance dashboard.** Recurring automated operations dashboard consolidating key metrics into a single leadership-facing view, with a supporting user guide. Refined across several review cycles based on direct executive feedback.
- **Vendor wind-down reporting.** Cross-functional dashboard tracking the wind-down of a major vendor relationship, giving leadership visibility into balance movement. Presented to the executive team.
- **Workers' compensation aged-inventory dashboard.** Co-led an analytics package quantifying aged balances, activity gaps, and compliance issues across multiple states and facilities.
- **Variance and underperformer analysis.** Leadership-facing summary covering variance-to-goal, collectible balances, and root-cause analysis for underperforming segments.
- **State-specific Medicaid write-off automation.** Two automated reports identifying accounts eligible for adjustment under state-specific billing rules, reducing manual research.
- **Payer-specific due diligence extension.** Extended the framework to a major national payer's secondary-account population, catching and fixing a data-accuracy issue mid-project before final findings.
- **Automated enrollment tracking.** Replaced manual tracking with a scheduled, validated report supporting timely follow-up on an enrollment-transition process.
- **Placement holds audit.** Reconciled charge, receipt, adjustment, insurance, and patient balance data at the account level to validate accuracy and support downstream billing decisions.
- **Closed-archive reconciliation report.** Built in DuckDB to catch accounts silently exiting active inventory without appearing on standard reconciliation files. A control-gap catch.
- **Daily automated duplicate payment report.** Triggered by posting-staff confirmation, giving leadership near real-time visibility into credit balance posting accuracy.

</details>

---

## Standards, Documentation, and Mentorship

Beyond individual reports, a few things that outlast any one deliverable.

I authored the business process team report layout standard, a reusable template the team has adopted across analyst work, and created the document audit guidelines that serve as a reference for audit procedure consistency. I also produced a 15-document technical package covering the full automated reporting portfolio, establishing reproducibility and handoff standards for the function.

I am currently onboarding and mentoring an analytics intern on audit procedures, cash posting review, and account resolution.

**Speaking.** Delivered two back-to-back presentations to groups of 50+ team members covering analytical findings, operational exposure, and workflow recommendations, both including live dashboard walkthroughs and Q&A with managers and senior staff. Completed a Train-the-Trainer program and delivered a 30-minute workflow-improvement presentation shared across leadership.

---

## Recognition

- Promoted to **Business Process Analyst III**, a role shaped in part around this body of work
- Trusted with near-full ownership of enterprise bad debt reporting across all facilities
- Bad debt pilot report selected for presentation up the leadership chain
- Reporting format adopted organization-wide
- Invited to present findings to leadership groups and a 100+ person cross-functional audience
- Recognized for visual design, clarity, and legibility, with same-day sign-off on delivered work

---

## What This Work Demonstrates

| Strength | Evidence |
|:---|:---|
| **Automation mindset** | Pipelines that refresh themselves and distribute on a schedule |
| **Data storytelling** | KPI structures, summaries, and visuals leadership actually reads |
| **Ownership** | Noticing problems and building the fix unasked, then being trusted with enterprise programs |
| **Collaboration** | Pulling AR, operations, vendor management, and IT into a shared view |
| **Measurable impact** | Cash accuracy, compliance visibility, refund routing accuracy, duplicate reduction |
| **Continuous improvement** | Substantial growth in R, DuckDB, and dashboard engineering over a short window |

<div align="center" markdown="1">

<a href="./"><img src="https://img.shields.io/badge/View_all_projects-1B365D?style=for-the-badge" alt="View all projects"></a>
<a href="./About.html"><img src="https://img.shields.io/badge/About_Me-1B365D?style=for-the-badge" alt="About"></a>

<sub>Employment work is described without proprietary figures, internal system names, or client-identifying detail.<br>
Specifics available in interview context.</sub>

</div>
