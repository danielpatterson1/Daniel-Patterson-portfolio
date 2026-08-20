<div align="center" markdown="1">

# U.S. Healthcare Costs, Payments, and Efficiency

**Interactive analytics dashboard built on the CMS National Health Expenditure Accounts**

<a href="U.S._Healthcare_Dashboard.html"><img src="https://img.shields.io/badge/Open_the_Dashboard-C9A227?style=for-the-badge" alt="Open dashboard"></a>
<a href="U.S._Healthcare_Report_RMD.Rmd"><img src="https://img.shields.io/badge/View_the_Code-1B365D?style=for-the-badge&logo=github&logoColor=white" alt="View code"></a>
<a href="./"><img src="https://img.shields.io/badge/←_Back_to_Portfolio-1B365D?style=for-the-badge" alt="Back to portfolio"></a>

<img src="https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white" alt="R">
<img src="https://img.shields.io/badge/flexdashboard-276DC3?style=flat-square" alt="flexdashboard">
<img src="https://img.shields.io/badge/plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white" alt="plotly">
<img src="https://img.shields.io/badge/CMS_NHEA-1B365D?style=flat-square" alt="CMS NHEA">

</div>

<br>

---

## Overview

The United States spends more per person on healthcare than any comparable country and does not get proportionally more health for it. That sentence gets repeated constantly and explains very little on its own.

This dashboard takes it apart. Using the CMS National Health Expenditure Accounts, the authoritative federal series on national health spending, it separates spending levels from spending growth, separates population-driven growth from per-person cost growth, and traces who actually pays for which services.

<div align="center" markdown="1">

| Annual national spending | Share of GDP | Publicly funded |
|:---:|:---:|:---:|
| **$5T+** | **~18%** | **~1/3** |

</div>

---

## Why It Was Built This Way

Healthcare spending is usually discussed one metric at a time. A headline per-capita figure, a GDP share, a growth rate. Each is true in isolation and misleading on its own, because the interesting questions live in how they interact.

The dashboard was designed around four separations that most summaries collapse:

| Separation | Why it matters |
|:---|:---|
| **Level vs. growth** | A category can be enormous and flat, or small and compounding fast. These call for entirely different responses |
| **Population vs. per-capita** | Spending more because there are more people is a different problem from spending more per person |
| **Nominal vs. real** | Without inflation adjustment, every long-run healthcare series looks like an emergency |
| **Service vs. payer** | Who pays varies sharply by service type, and the aggregate payer mix hides that |

> This dashboard is exploratory and analytical. It describes what the spending data shows and does not make policy recommendations.

---

## Key Findings

**Spending rises structurally, not cyclically.** National health expenditure exceeds $5T annually and sits near 18% of GDP. The upward trend persists after inflation adjustment, which rules out price-level effects as the explanation.

**Per-person cost is the engine, not population.** Decomposing total growth shows that higher cost per person accounts for most of the increase. Population growth contributes meaningfully less. This is the single most useful finding in the dashboard, because it redirects attention from demographics to unit cost.

**Spending is highly concentrated.** Hospital care and physician and clinical services dominate the total, and a small number of categories drive most incremental growth. Concentration is what makes the problem tractable: a few categories carry most of the movement.

**Public programs carry a growing share.** Medicare and Medicaid together fund roughly a third of total spending, and payment responsibility varies widely by service type. The aggregate figure conceals how differently a hospital stay and a prescription are financed.

**Costs outpace income.** Spending per person has grown faster than GDP per capita, and the gap between the two continues to widen. This is the affordability finding, and it is the one that compounds.

---

## How to Read the Dashboard

| View | What it answers |
|:---|:---|
| **Summary metrics** | Snapshot of cost levels, growth rates, and funding mix |
| **Time series** | How spending has moved, nominal against inflation-adjusted |
| **Growth decomposition** | How much growth comes from population versus cost per person |
| **Service-level analysis** | Which categories hold the spending and which drive the growth |
| **Payer views** | How Medicare, Medicaid, private insurance, and out-of-pocket split the bill |

Interactive controls filter by time horizon and metric, so each view can be narrowed to a specific era rather than read only in aggregate.

---

## Data and Method

| Element | Detail |
|:---|:---|
| **Source** | CMS National Health Expenditure Accounts (NHEA) |
| **Coverage** | Total spending, per-capita spending, payer mix, GDP, population |
| **Inflation adjustment** | Historical CPI indices applied to produce real-terms series |
| **Validation** | Cross-checked across multiple CMS tables for internal consistency |
| **Build** | R with the tidyverse, flexdashboard for layout, plotly for interactivity |

---

## Limitations

These bound what the dashboard can be used for.

**Spending is not outcomes.** NHEA measures dollars, not health. Nothing here supports a claim about whether the spending buys value, only about where it goes.

**Efficiency is inferred, not measured.** The efficiency views compare spending growth against population and income growth. That is a useful proxy and not a productivity measure. A true efficiency metric would need service volume and outcome data the NHEA does not carry.

**National aggregates hide variation.** State, regional, and institutional differences are substantial and invisible at this level of aggregation.

**Categories shift over time.** CMS has revised service category definitions across the history of the series, so very long-run comparisons within a single category carry some definitional drift.

---

## What I Would Add Next

State-level expenditure data to expose the geographic variation the national series flattens, and an international comparison against OECD health spending to put the GDP share in context rather than leaving it as a standalone number.

<div align="center" markdown="1">

<a href="U.S._Healthcare_Dashboard.html"><img src="https://img.shields.io/badge/Open_the_Dashboard-C9A227?style=for-the-badge" alt="Open dashboard"></a>
<a href="./"><img src="https://img.shields.io/badge/All_Projects-1B365D?style=for-the-badge" alt="All projects"></a>

<sub>Built on public CMS data. Analysis and interpretation are my own.</sub>

</div>
