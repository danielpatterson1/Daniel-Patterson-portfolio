# Work Wins & Case Studies

Analytics • Automation • Operational Reporting • Data Storytelling
Updated: July 2026

## Executive Summary

Over the last two years I've built out analytics, automation, and reporting improvements that made financial data more accurate, got insights in front of leadership faster, and gave operations tighter control across credit balance, Medicaid AR, bad debt, and refund reconciliation work.

In 2026 I was promoted to Business Process Analyst III and given near-full ownership of enterprise-wide bad debt and underperformer reporting across all facilities. The flagship bad debt report is slated for the BSO Director to present up to her own leadership.

The work that stands out most:

- Enterprise bad debt reporting program — quarter-over-quarter improvement tracking and clean-up targeting, piloted at one hospital and now being extended into a dedicated report for every facility in the network.
- Underperformers reporting — an all-facility view of operational risk, with a team-level version in progress for more targeted coaching.
- Automated refund accuracy report — cross-team reconciliation of refund recipients against the current vendor list, running on a scheduled, automated distribution to AR teams.
- Credit Balance Operational Report — the department-standard dashboard covering inventory, dollars, team throughput, compliance, and timing.
- Duplicate payment review — surfaced $3.62M in duplicates and supported a ~60% month-over-month reduction.
- Due Diligence Initiative — a self-initiated review that cleared hundreds of thousands of dollars in stalled balances from the active worklist, and later extended into an automated Medicaid Due Diligence Report ($671K in actionable backlog in month one, ~$1M in write-offs projected).
- Automated credit balance reporting suite — one-click HTML reporting that cut refresh time and error risk.
- Medicaid AR HTML report — pinpointed the payer segments, aging patterns, and payment-timing delays driving the most operational risk.

Taken together, the through-line is measurable financial impact, scalable automation, cross-functional collaboration, clear storytelling, and reporting design that leadership actually adopts.

---

## Enterprise Bad Debt Reporting Program

The goal here is to give hospital leadership a clean, repeatable read on bad debt — how it's trending quarter over quarter, where the biggest clean-up opportunities sit, and which segments are driving the picture. It started as a single-hospital pilot, and the structure and visual language were designed from the start to translate cleanly to every other facility.

The pilot proved out well enough that I was picked to take near-full ownership of the program, and the finished report is going up the chain: the BSO Director is presenting it to her leadership. From there, it becomes a recurring per-facility product across the network.

## Underperformers Reporting Suite

Same idea, different lens. Leadership needed a way to see where operational performance was drifting early enough to act, so I built an all-facility underperformers report that surfaces the risk segments across the network. A team-level version is in progress now — same framework, but granular enough for managers to coach against.

## Automated Refund Accuracy Report

There was a recurring gap where refunds were occasionally being mailed to outdated vendor addresses, because manual matching couldn't keep up with vendor-file changes. I built cross-team reconciliation logic that matches refund recipients against the current vendor list of record, and put it on an automated distribution schedule to AR teams. No more manual pull, no manual review handoff — and the misdirected-refund risk went with it.

---

## Flagship Project — Credit Balance Operational Report

The Credit Balance Operational Report was built to give the department a single, honest picture of credit balance activity: monthly and weekly trends, decentralized vs. centralized comparisons, team throughput, payer drivers, and compliance timing.

The design choices matter here. Daily-average inventory and dollars smooth out noise so trends are readable. Team drilldowns let managers see accounts, dollars, payer mix, and throughput at their own level. There's a pre/post view around a major operational restructuring, a weekly lens for catching inflow shifts and timing outliers, and responsible-party insights that show when a payer is driving the numbers.

It ended up becoming the department-wide standard layout and was called out for clarity, visual design, and legibility. It also introduced the Executive Summary + KPI Box format that's now used across other departmental reports.

## Duplicate Payment Review — $3.62M Identified

The objective was straightforward: find the duplicate payments, figure out what was causing them, quantify the exposure, and drive remediation.

The review surfaced $3.62M in duplicates — roughly 60% from delayed insurance postings, 28% from automatic-posting errors, and 12% from cash-posting errors. On the fix side, we improved EDI response tracking, extended the posting-delay threshold to cut down false-duplicate flags, tightened detection logic, and added QA checks around large batches.

The result was a ~60% month-over-month reduction in duplicates and a clean downward trend after remediation. The segment-level breakdown also gave the team something concrete to build targeted training around. Department leadership called it out for clarity and rigor.

I was then picked to present the findings to a cross-functional audience of 100+ team members — financial exposure, root causes, the dashboards, and the process changes behind the reduction. The work later got featured in an internal company-wide recognition program highlighting analyst contributions.

## Due Diligence Initiative

This one wasn't assigned. I noticed a recurring pattern of stalled, unresolved balances sitting on the active worklist while doing day-to-day operational work, and built a review process to systematically work through them.

The process included a repeatable review flow to flag and resolve aged worklist balances, a documented process map, and an automated reporting solution. Filters and payer-classification logic went through several rounds of stakeholder feedback before it landed.

It recovered hundreds of thousands of dollars in outstanding balances, moved to daily automated distribution with zero calculation errors during team review, and got adopted as an ongoing operational process rather than a one-off.

The framework carried forward. In 2026 I built an automated Medicaid Due Diligence Report on top of it that surfaced $671K in actionable backlog within its first month and is projected to support around $1M in write-offs overall.

---

## Additional Reporting & Leadership Briefings

A handful of other operational reports I've built and put in front of senior leadership:

- **Medicaid Performance Dashboard** — a recurring, automated Medicaid operations dashboard that consolidates key metrics into a single leadership-facing view, with a supporting user guide. Refined across several review cycles based on direct executive feedback.
- **Vendor Account Wind-Down Reporting** — a cross-functional dashboard tracking the wind-down of a major vendor relationship, giving leadership clear visibility into balance movement. Presented to the executive team; positive feedback.
- **Variance & Underperformer Analysis** — a leadership-facing summary covering variance-to-goal, collectible balances, and root-cause analysis for underperforming segments. The executive summary framework got specific praise, and it's since been extended into the standalone underperformers suite mentioned above.
- **Payer-Specific Due Diligence Extension** — extended the Due Diligence framework to a major national payer's secondary-account population; caught and fixed a data-accuracy issue mid-project before presenting final findings.
- **Automated Enrollment-Tracking Report** — replaced manual tracking with a scheduled, validated report supporting timely follow-up on an enrollment-transition process.
- **OHPAC Placement Holds Audit** — reconciled charge, receipt, adjustment, insurance, and patient balance data at the account level to validate accuracy and support downstream billing decisions.
- **Revco Closed Archive Report** — built in DuckDB to catch accounts silently exiting active inventory without appearing on standard reconciliation files. A control-gap catch.
- **Daily Automated Duplicate Payment Report** — triggered by posting-staff confirmation, giving executive leadership near real-time visibility into credit balance posting accuracy.

## Documentation & Standards

Beyond the reports themselves, I've contributed a few things that outlast any one deliverable. I authored the BSO Business Process Team report layout standard — a reusable template that the team has adopted across analyst work. I also created and presented the Document Manager Audit Guidelines, which serve as a reusable reference for audit procedure consistency. And I'm actively onboarding and mentoring an analytical intern on audit procedures, cash posting review, and account resolution.

## Speaking & Presentation Highlights

In 2025 I delivered two back-to-back presentations to groups of 50+ team members covering analytical findings, operational exposure, and workflow recommendations. Both included live dashboard walkthroughs and Q&A with managers and senior staff. Got recognized for clarity, composure, and communication.

## Training & Certification

Completed a Train-the-Trainer program and delivered a 30-minute workflow-improvement presentation that was shared across leadership and the broader team.

---

## Automated Credit Balance Reporting Suite

A fully automated R/HTML reporting pipeline consolidating operational credit-balance metrics — balance-tier breakdowns, facility-level analytics, responsible-party insights, team workflows (accounts, compliance, aging), and aging buckets tied to operational status. One-click refresh, lower error risk, faster cadence, and a reusable framework I've built other reports on top of since. Direct feedback: "Strong design and legibility."

## Medicaid AR HTML Report

Built to analyze Medicaid AR and find where balance concentration, plan-level delays, and operational risk were actually sitting.

What came out of it: balances were concentrated in a small number of high-volume facility groups; a handful of payer plan codes accounted for a disproportionate share of the impact; select segments were seeing discharge-to-payment delays of 400–580+ days; and payments were concentrated within a specific high-volume claim series.

The report gave the team targeted insights for follow-up, clear segmentation to guide operations, an auto-refresh capability, and expanded visibility into plan-level payment behavior that wasn't there before.

---

## Leadership Recognition

- Promoted to Business Process Analyst III — the role was shaped in part around this body of work.
- Trusted with near-full ownership of enterprise bad debt reporting across all facilities.
- Bad debt pilot report selected for the BSO Director to present up to her leadership.
- Reporting format adopted organization-wide.
- Recognized for standout visuals and clarity.
- Invited to present findings to leadership groups.
- Commended publicly for graph design.
- Train-the-Trainer presentation praised.

## Core Strengths Demonstrated

Automation mindset — pipelines that refresh themselves and distribute on a schedule. Data storytelling — KPIs, summaries, and visuals that people can actually read. Ownership — noticing things and building the fix without being asked, and being trusted with enterprise programs as a result. Collaboration — pulling AR, operations, vendor management, and IT into the same view. Impact — cash accuracy, compliance visibility, refund routing accuracy. Continuous improvement — real growth in R, DuckDB, and dashboard engineering over a short window.

## Impact Summary

- Promoted to Business Process Analyst III; entrusted with near-full ownership of enterprise bad debt and underperformer reporting across all facilities.
- Identified $3.62M in duplicate payments and supported a ~60% reduction.
- Automated Medicaid Due Diligence Report surfaced $671K in actionable backlog within its first month, with ~$1M in write-offs projected overall.
- Ran a self-initiated Due Diligence process that recovered hundreds of thousands of dollars from the worklist.
- Delivered an enterprise credit balance operational report that became the department standard.
- Built automated pipelines — including cross-team refund reconciliation — that cut refresh time, removed manual handoffs, and reduced error risk.
- Scaled reporting frameworks across multiple operational areas.
- Consistently recognized for clarity, design standards, and operational value.
