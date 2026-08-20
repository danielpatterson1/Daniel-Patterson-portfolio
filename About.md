<div align="center">

# Daniel Patterson

### Business Process Analyst III
**Healthcare Revenue Cycle Analytics · Reporting Automation · Statistical Analysis**

<a href="https://www.linkedin.com/in/daniel-patterson-b03a5718b"><img src="https://img.shields.io/badge/LinkedIn-Connect-1B365D?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="https://github.com/danielpatterson1"><img src="https://img.shields.io/badge/GitHub-Follow-1B365D?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"></a>
<a href="mailto:dpatterson6575@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-1B365D?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
<a href="Daniel_Patterson_Resume.pdf"><img src="https://img.shields.io/badge/Resume-Download-C9A227?style=for-the-badge&logo=readthedocs&logoColor=white" alt="Resume"></a>

<br>

<img src="https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white" alt="R">
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=microsoftsqlserver&logoColor=white" alt="SQL">
<img src="https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black" alt="DuckDB">
<img src="https://img.shields.io/badge/Quarto-75AADB?style=flat-square&logo=quarto&logoColor=white" alt="Quarto">
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git">

<br>

*I build automated reporting pipelines and operational dashboards for healthcare revenue cycle teams,<br>
and run independent analysis on public health and safety datasets.*

**M.S. Analytics, Georgia Tech** · Computational Data Analytics track · Expected December 2028

</div>

<br>

---

## Project Index

| Project | What it does | Deliverable |
|:---|:---|:---|
| **Medicare Payment Variability** | Benchmarks 2,845 providers against DRG-level peer norms to flag where charges and payments decouple | [View dashboard](Healthcare_Revenue_Leakage_Recovery_Model.html) |
| **U.S. Healthcare Cost & Efficiency** | Traces six decades of national spending, payer mix shifts, and where the cost growth actually sits | [View dashboard](U.S._Healthcare_Dashboard.html) |
| **Tesla Fatal Crash Involvement** | Tests an adverse-weather safety hypothesis against 37,654 fatal crashes, and shows why it fails | [View report](./tesla-report.html) |
| **Work Wins & Case Studies** | Production analytics at enterprise scale | [View write-ups](./Work-wins.md) |
| **About Me** | Background and technical stack | [Read more](./About.md) |

<br>

---

## 💵 Medicare Payment Variability

### Revenue Leakage Detection Model

<img src="https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white" alt="R">
<img src="https://img.shields.io/badge/Quarto-75AADB?style=flat-square&logo=quarto&logoColor=white" alt="Quarto">
<img src="https://img.shields.io/badge/CMS_Claims-1B365D?style=flat-square" alt="CMS Claims">
<img src="https://img.shields.io/badge/Peer_Benchmarking-1B365D?style=flat-square" alt="Peer Benchmarking">
<img src="https://img.shields.io/badge/Outlier_Detection-1B365D?style=flat-square" alt="Outlier Detection">

Hospitals billing the same DRG do not get paid the same way. Some of that spread is legitimate: case mix, wage index, teaching status, outlier payments. Some of it is not, and the difference is where payment integrity teams make their money.

This model separates the two. It benchmarks **2,845 providers** against DRG-level peer norms, measures how far each provider's charge-to-payment relationship departs from its comparison group, and ranks the resulting gaps so the largest and most anomalous rise to the top of a work queue.

<div align="center">

| Providers benchmarked | Variance exposure identified | Concentration |
|:---:|:---:|:---:|
| **2,845** | **$8.2B** | **Top 10 providers** |

</div>

**How the model works:**

| Step | What it does |
|:---|:---|
| DRG-level peer grouping | Compares each provider only against hospitals billing the same procedure, so case mix does not masquerade as anomaly |
| Charge-to-payment decoupling | Measures where submitted charges and realized Medicare payments move independently rather than together |
| Variance decomposition | Separates spread that DRG and provider characteristics explain from spread that they do not |
| Outlier ranking | Scores and sorts providers by departure from peer norm, producing a prioritized review list |
| Concentration analysis | Establishes that exposure is heavily top-loaded rather than evenly spread, which is what makes it actionable |

> **On what exposure means.** Exposure is a screening signal that flags where payment patterns diverge from peer norms. It is not a recovery estimate. Converting any share of it into recoverable revenue would require claim-level adjudication data the public files do not contain. The value of the model is triage: it tells you which 10 providers to look at first out of 2,845, not what you will collect.

**Why it matters:** this is the same shape of problem payment integrity vendors and payer SIU teams solve daily. The exercise here was building the screening layer end to end on public data, including the discipline of labeling the output as a lead list rather than a recovery forecast.

**[Open the dashboard →](Healthcare_Revenue_Leakage_Recovery_Model.html)**

<br>

---

## 🏥 U.S. Healthcare Cost, Payments, and Efficiency

<img src="https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white" alt="R">
<img src="https://img.shields.io/badge/plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white" alt="plotly">
<img src="https://img.shields.io/badge/CMS_NHE-1B365D?style=flat-square" alt="CMS NHE">
<img src="https://img.shields.io/badge/Time_Series-1B365D?style=flat-square" alt="Time Series">
<img src="https://img.shields.io/badge/Interactive-1B365D?style=flat-square" alt="Interactive">

The United States spends more per person on healthcare than any comparable country and does not get proportionally more health for it. This dashboard works through where that money actually goes, using the CMS National Health Expenditure accounts, the authoritative federal series on national health spending.

Rather than restating the headline per-capita number, the dashboard decomposes it: which categories of care drive the total, which payers absorb the cost, how the mix has shifted across decades, and where growth has accelerated against where it has flattened.

**What the dashboard covers:**

| View | Question it answers |
|:---|:---|
| Spending trends | How has national health expenditure grown over time in absolute terms, per capita, and as a share of GDP? |
| Category breakdown | How much goes to hospital care, physician and clinical services, prescription drugs, and administration? |
| Payer mix | How has the split between Medicare, Medicaid, private insurance, and out-of-pocket spending shifted? |
| Growth decomposition | Which categories are accelerating, which have flattened, and where is the compounding actually happening? |
| Efficiency measures | Where does spending growth outpace the growth in services delivered? |

> **Why the payer mix view matters most.** Aggregate spending totals get quoted constantly and explain very little. The payer decomposition is the part that changes how you read the rest of the series, because it shows who absorbs each additional dollar and therefore who has the incentive to control it.

Built in R with interactive plotly charts, so every series can be filtered, hovered, and inspected rather than read as a static image.

**[Open the dashboard →](U.S._Healthcare_Dashboard.html)** · [Executive summary](U.S._Healthcare_README.md) · [Source code](U.S._Healthcare_Report_RMD.Rmd)

<br>

---

## 🚗 Tesla Fatal Crash Involvement

### Geography, Weather, and Exposure · NHTSA FARS 2023

<img src="https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white" alt="R">
<img src="https://img.shields.io/badge/Quarto-75AADB?style=flat-square&logo=quarto&logoColor=white" alt="Quarto">
<img src="https://img.shields.io/badge/Logistic_Regression-1B365D?style=flat-square" alt="Logistic Regression">
<img src="https://img.shields.io/badge/Power_Analysis-1B365D?style=flat-square" alt="Power Analysis">

Tests whether Tesla vehicles are disproportionately involved in fatal crashes during adverse weather, using all 37,654 fatal crashes in the 2023 FARS file.

> **The headline result is a null.** Raw figures suggest a rain effect. It does not survive testing. The association is not statistically distinguishable from zero, it is fully consistent with the geographic concentration of the Tesla fleet in warm states that get rain and little snow, and it is smaller than the available sample could reliably detect.

**What the analysis does to establish that:**

| Method | Purpose |
|:---|:---|
| Logistic regression, state fixed effects | Separates a weather signal from fleet geography |
| Single-state sensitivity check | Holds climate and road network constant by construction |
| Wilson score intervals | "Above baseline" means resolvable, not just numerically different |
| Minimum detectable effect | Bounds the null instead of leaving it ambiguous |
| Model-year hardware split | Tests the camera-only mechanism claim on its own terms |
| Inline-generated figures | No number in the prose can drift from the code behind it |

**[Read the full report →](./tesla-report.html)**

<br>

---

## 🧾 Work Wins & Case Studies

Production analytics work, summarized without proprietary figures. Specifics available on request.

<details>
<summary><b>Expand full list</b></summary>

<br>

**Enterprise cash reconciliation platform**
Reconciles deposits against posting activity at a 98.5% match rate across roughly a billion dollars in annual volume. Surfaced a multi-million-dollar auto-posting break that manual review had not caught.

**Bad debt write-off reporting program**
Parameterized pipeline generating facility-level dashboards across 170+ hospitals from a single source file, extended into a region-level roll-up for Regional Controllers.

**Duplicate payment detection**
Identified duplicate payment exposure at roughly 99% precision and drove a ~60% month-over-month reduction in recurrence through payer and day-trend root cause analysis.

**Due Diligence write-off automation**
Automated Medicaid, BCBS, and QMB workflows supporting seven figures in substantiated write-offs within the first month of deployment.

**Underperformers reporting**
All-facility and team-level scorecards used by operations leadership.

**Credit balance and Medicaid AR reporting suite**
Recurring operational reporting with scheduled distribution.

</details>

**[Full write-ups →](./Work-wins.md)**

<br>

---

## 🛠 Technical Stack

| Area | Tools |
|:---|:---|
| **Languages** | R, Python, SQL |
| **Data** | DuckDB, SQL Server, dplyr, pandas |
| **Reporting** | Quarto, RMarkdown, flexdashboard, ggplot2, plotly |
| **Statistics** | Logistic regression, hypothesis testing, power analysis, uncertainty quantification |
| **Workflow** | Git, parameterized pipelines, automated scheduling |

<br>

---

<div align="center">

### Get in touch

<a href="https://www.linkedin.com/in/daniel-patterson-b03a5718b"><img src="https://img.shields.io/badge/LinkedIn-1B365D?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="mailto:dpatterson6575@gmail.com"><img src="https://img.shields.io/badge/Email-1B365D?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
<a href="https://github.com/danielpatterson1"><img src="https://img.shields.io/badge/GitHub-1B365D?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"></a>

<sub>Independent projects use public datasets (CMS, NHTSA FARS) and reflect my own analysis.<br>
Employment work is summarized without proprietary figures.</sub>

</div>- Delivered the **Medicaid AR HTML dashboard** for high‑risk plan analysis.
- Introduced a new **Executive Summary + KPI layout** now standard in multiple departmental reports.
- Presented a **cash posting document management solution** to assistant director and IT leadership.

---

## 🎓 Currently Learning

- Pursuing an **M.S. in Analytics (OMSA)** at the **Georgia Institute of Technology** — in progress, degree conferral expected December 2028.

---

## 📬 Contact Me

**LinkedIn:**
[https://www.linkedin.com/in/daniel-patterson-b03a5718b/](https://www.linkedin.com/in/daniel-patterson-b03a5718b/)

**Email:** [dpatterson6575@gmail.com](mailto:dpatterson6575@gmail.com)

Thanks for visiting my portfolio!
