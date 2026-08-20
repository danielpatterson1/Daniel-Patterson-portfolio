<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>About · Daniel Patterson</title>
<meta name="description" content="Daniel Patterson, Business Process Analyst III. Healthcare revenue cycle analytics, reporting automation, and statistical analysis.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Newsreader:ital,opsz,wght@0,6..72,400;0,6..72,500;0,6..72,600;1,6..72,400&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
:root{
  --navy:#1B365D;
  --navy-deep:#12243D;
  --gold:#C9A227;
  --gold-soft:#FFFDF3;
  --ink:#111827;
  --body:#3A4658;
  --muted:#6B7688;
  --rule:#E4E7EC;
  --paper:#FFFFFF;
  --tint:#F7F8FA;
  --display:"Newsreader",Georgia,"Times New Roman",serif;
  --sans:"Inter",-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,sans-serif;
}

*{box-sizing:border-box;}
html{-webkit-text-size-adjust:100%;}
body{
  margin:0;
  background:var(--paper);
  color:var(--body);
  font-family:var(--sans);
  font-size:16.5px;
  line-height:1.7;
  -webkit-font-smoothing:antialiased;
}
.wrap{max-width:840px;margin:0 auto;padding:0 1.5rem;}

/* ---------- Masthead ---------- */
.masthead{
  background:var(--navy);
  background-image:linear-gradient(160deg,var(--navy) 0%,var(--navy-deep) 100%);
  color:#fff;
  padding:3.6rem 0 3rem;
  border-bottom:4px solid var(--gold);
}
.masthead .eyebrow{
  font-size:.7rem;font-weight:700;letter-spacing:.18em;text-transform:uppercase;
  color:var(--gold);margin:0 0 1rem;
}
.masthead h1{
  font-family:var(--display);
  font-size:clamp(2.4rem,6vw,3.4rem);
  font-weight:500;line-height:1.05;letter-spacing:-.02em;
  margin:0 0 .5rem;color:#fff;
}
.masthead .role{
  font-size:1.05rem;color:#C7D2E1;margin:0 0 .35rem;font-weight:500;
}
.masthead .disciplines{
  font-size:.9rem;color:#8FA3BC;margin:0 0 1.9rem;letter-spacing:.01em;
}
.btnrow{display:flex;flex-wrap:wrap;gap:.6rem;}
.btn{
  display:inline-block;font-size:.8rem;font-weight:600;letter-spacing:.03em;
  padding:.6rem 1.05rem;border-radius:2px;text-decoration:none;
  border:1px solid rgba(255,255,255,.32);color:#fff;
  transition:background .15s ease,border-color .15s ease,color .15s ease;
}
.btn:hover{background:rgba(255,255,255,.12);border-color:rgba(255,255,255,.6);}
.btn-gold{background:var(--gold);border-color:var(--gold);color:var(--navy-deep);}
.btn-gold:hover{background:#DDB63A;border-color:#DDB63A;color:var(--navy-deep);}

/* ---------- Sections ---------- */
section{padding:3.2rem 0 .6rem;}
section + section{border-top:1px solid var(--rule);}
.label{
  font-size:.68rem;font-weight:700;letter-spacing:.16em;text-transform:uppercase;
  color:var(--gold);margin:0 0 .5rem;
}
h2{
  font-family:var(--display);font-size:1.85rem;font-weight:500;
  color:var(--ink);letter-spacing:-.015em;margin:0 0 1.2rem;line-height:1.2;
}
h3{
  font-size:.95rem;font-weight:700;color:var(--navy);
  margin:1.8rem 0 .3rem;letter-spacing:.01em;
}
p{margin:0 0 1.1rem;}
a{color:var(--navy);text-decoration:none;border-bottom:1px solid rgba(27,54,93,.28);}
a:hover{color:var(--gold);border-bottom-color:var(--gold);}

/* ---------- Caveat block: the page's signature ---------- */
.caveat{
  background:var(--gold-soft);
  border-left:3px solid var(--gold);
  padding:1.3rem 1.5rem;
  margin:1.8rem 0;
}
.caveat .k{
  display:block;font-size:.68rem;font-weight:700;letter-spacing:.14em;
  text-transform:uppercase;color:#8A6D12;margin-bottom:.5rem;
}
.caveat p{margin:0;font-size:.96rem;color:#4A4433;}

/* ---------- Definition rows ---------- */
.rows{border-top:1px solid var(--rule);margin:1.4rem 0 0;}
.row{
  display:grid;grid-template-columns:210px 1fr;gap:1.5rem;
  padding:.95rem 0;border-bottom:1px solid var(--rule);align-items:start;
}
.row dt{font-weight:600;color:var(--ink);font-size:.9rem;padding-top:.1rem;}
.row dd{margin:0;font-size:.93rem;color:var(--body);}

/* ---------- Ledger: highlights with the figure pulled out ---------- */
.ledger{margin:1.4rem 0 0;border-top:1px solid var(--rule);}
.entry{
  display:grid;grid-template-columns:1fr 132px;gap:1.5rem;
  padding:1.15rem 0;border-bottom:1px solid var(--rule);align-items:baseline;
}
.entry .what{margin:0;}
.entry .what b{display:block;color:var(--ink);font-weight:650;font-size:.95rem;margin-bottom:.2rem;}
.entry .what span{font-size:.9rem;color:var(--body);}
.entry .fig{
  text-align:right;font-family:var(--display);font-size:1.5rem;font-weight:500;
  color:var(--navy);line-height:1.1;font-variant-numeric:tabular-nums;
}
.entry .fig small{
  display:block;font-family:var(--sans);font-size:.64rem;font-weight:700;
  letter-spacing:.1em;text-transform:uppercase;color:var(--muted);margin-top:.3rem;
}

/* ---------- Education ---------- */
.edu{padding:1.1rem 0;border-bottom:1px solid var(--rule);}
.edu:first-of-type{border-top:1px solid var(--rule);margin-top:1.4rem;}
.edu b{color:var(--ink);font-size:.98rem;font-weight:650;}
.edu .inst{color:var(--body);font-size:.93rem;}
.edu .meta{color:var(--muted);font-size:.85rem;}

/* ---------- Footer ---------- */
footer{
  background:var(--tint);border-top:1px solid var(--rule);
  margin-top:3.4rem;padding:2.8rem 0;
}
footer h2{font-size:1.35rem;margin-bottom:1rem;}
footer .btn{border-color:rgba(27,54,93,.3);color:var(--navy);}
footer .btn:hover{background:var(--navy);border-color:var(--navy);color:#fff;}
footer .fine{
  font-size:.8rem;color:var(--muted);margin:1.6rem 0 0;line-height:1.6;
}

a:focus-visible,.btn:focus-visible{outline:2px solid var(--gold);outline-offset:3px;}
@media (prefers-reduced-motion:reduce){*{transition:none!important;}}

@media (max-width:640px){
  .row,.entry{grid-template-columns:1fr;gap:.35rem;}
  .entry .fig{text-align:left;font-size:1.35rem;}
  .entry .fig small{margin-top:.1rem;}
  section{padding:2.4rem 0 .5rem;}
  .masthead{padding:2.6rem 0 2.2rem;}
}
</style>
</head>
<body>

<header class="masthead">
  <div class="wrap">
    <p class="eyebrow">About</p>
    <h1>Daniel Patterson</h1>
    <p class="role">Business Process Analyst III</p>
    <p class="disciplines">Analytics automation · Operational reporting · Statistical analysis</p>
    <div class="btnrow">
      <a class="btn" href="./">All projects</a>
      <a class="btn btn-gold" href="Daniel_Patterson_Resume.pdf">Resume</a>
      <a class="btn" href="https://www.linkedin.com/in/daniel-patterson-b03a5718b">LinkedIn</a>
      <a class="btn" href="mailto:dpatterson6575@gmail.com">Email</a>
    </div>
  </div>
</header>

<main class="wrap">

<section>
  <p class="label">What I do</p>
  <h2>Reporting systems for revenue cycle operations</h2>
  <p>I work where finance, operations, and data meet: reconciling cash, surfacing payment errors, and putting numbers in front of controllers and directors before they have to ask for them.</p>
  <p>Most of what I build replaces something that used to be done by hand. A recurring report that took a day of copying and filtering becomes a parameterized pipeline that runs on a schedule and produces the same output for 170 facilities at once. That shift is the throughline of my work.</p>

  <div class="caveat">
    <span class="k">What I care about beyond throughput</span>
    <p>Automation is only useful if the output is right, and the harder discipline is knowing when a number does not mean what it appears to mean. A large figure with no denominator. A significant p-value on a trivial effect size. A difference that turns out to be a difference in exposure. Building reports that resist those mistakes matters more to me than building them fast.</p>
  </div>
</section>

<section>
  <p class="label">Strengths</p>
  <h2>What I am best at</h2>
  <dl class="rows">
    <div class="row"><dt>Automation</dt><dd>Converting recurring manual reporting into parameterized pipelines that run unattended and scale across facilities without additional effort.</dd></div>
    <div class="row"><dt>Operational analytics</dt><dd>Cash reconciliation, credit balances, Medicaid AR, bad debt write-offs, duplicate payment detection, and payment variability analysis.</dd></div>
    <div class="row"><dt>Statistical rigor</dt><dd>Uncertainty quantification, confounder adjustment, and knowing the limits of what a given dataset can support.</dd></div>
    <div class="row"><dt>Report design</dt><dd>Clean, consistent HTML reporting frameworks with a shared design language across a full portfolio of reports.</dd></div>
    <div class="row"><dt>Data storytelling</dt><dd>KPI structures and visuals that leadership uses to make decisions, not just to acknowledge.</dd></div>
    <div class="row"><dt>Cross-functional work</dt><dd>Translating between operations teams who know the process and technical teams who know the data.</dd></div>
  </dl>
</section>

<section>
  <p class="label">Toolkit</p>
  <h2>Technical skills</h2>
  <dl class="rows">
    <div class="row"><dt>Languages</dt><dd>R, SQL, Python</dd></div>
    <div class="row"><dt>Data</dt><dd>DuckDB, SQL Server, dplyr, tidyr, pandas</dd></div>
    <div class="row"><dt>Visualization</dt><dd>ggplot2, plotly, flexdashboard, Power BI (working knowledge)</dd></div>
    <div class="row"><dt>Reporting</dt><dd>Quarto, R Markdown, HTML, CSS, parameterized rendering</dd></div>
    <div class="row"><dt>Statistics</dt><dd>Logistic regression, hypothesis testing, power analysis, confounder adjustment, uncertainty quantification</dd></div>
    <div class="row"><dt>Workflow</dt><dd>Git, GitHub Pages, scheduled distribution, reproducible pipelines</dd></div>
  </dl>
</section>

<section>
  <p class="label">Education</p>
  <h2>Background</h2>
  <div class="edu">
    <b>M.S. Analytics</b><br>
    <span class="inst">Georgia Institute of Technology</span><br>
    <span class="meta">Computational Data Analytics track · Expected December 2028</span>
  </div>
  <div class="edu">
    <b>B.A. Economics and Econometrics</b><br>
    <span class="inst">University of South Florida</span><br>
    <span class="meta">December 2024</span>
  </div>
  <div class="edu">
    <b>Google Data Analytics Certificate</b><br>
    <span class="meta">2025</span>
  </div>
</section>

<section>
  <p class="label">Selected work</p>
  <h2>Recent highlights</h2>
  <p>Promoted to Business Process Analyst III, a role shaped in part by the automation work below.</p>
  <div class="ledger">
    <div class="entry">
      <p class="what"><b>Enterprise cash reconciliation platform</b><span>Matches deposits against payment-posting activity across roughly a billion dollars in annual volume, and surfaced a multi-million-dollar auto-posting break that manual review had not caught.</span></p>
      <p class="fig">98.5%<small>Match rate</small></p>
    </div>
    <div class="entry">
      <p class="what"><b>Regional bad debt write-off reporting</b><span>Converted a facility-level dashboard into a seven-page regional roll-up for Regional Controllers, consolidating write-off drivers, facility scorecards, and operational watchlists.</span></p>
      <p class="fig">170+<small>Facilities</small></p>
    </div>
    <div class="entry">
      <p class="what"><b>Due diligence automation</b><span>Automated Medicaid, BCBS, and QMB overpayment identification, supporting seven figures in substantiated write-offs within the first month live.</span></p>
      <p class="fig">3<small>Workflows</small></p>
    </div>
    <div class="entry">
      <p class="what"><b>Duplicate payment detection</b><span>Identified duplicate payment exposure at roughly 99% precision and supported a sustained reduction through payer and day-trend root cause analysis.</span></p>
      <p class="fig">~60%<small>Reduction</small></p>
    </div>
    <div class="entry">
      <p class="what"><b>Documentation program</b><span>Authored a technical package covering the full automated reporting portfolio, establishing reproducibility and handoff standards for the function.</span></p>
      <p class="fig">15<small>Documents</small></p>
    </div>
    <div class="entry">
      <p class="what"><b>Credit Balance Operational Report</b><span>Designed and deployed enterprise-wide.</span></p>
      <p class="fig">2025<small>Deployed</small></p>
    </div>
  </div>
</section>

<section>
  <p class="label">Outside work</p>
  <h2>Independent projects</h2>
  <p>I analyze public datasets partly to stay sharp on methods I do not use daily.</p>

  <h3>Medicare Payment Variability Model</h3>
  <p>Benchmarks 2,845 providers against DRG-level peer norms and surfaces $8.2B in payment variance exposure, built entirely on public CMS files.</p>

  <h3>Tesla Fatal Crash Involvement Analysis</h3>
  <p>Tests whether Teslas are over-involved in adverse-weather fatal crashes across 37,654 records in the NHTSA FARS file. The interesting part is that the answer is no. An apparent rain effect turns out to be geographic confounding, and the report quantifies how small an effect the data could actually have detected. Finding and dismantling my own promising result taught me more than confirming one would have.</p>

  <p style="margin-top:1.6rem;"><a href="./">See all projects</a></p>
</section>

</main>

<footer>
  <div class="wrap">
    <h2>Get in touch</h2>
    <div class="btnrow">
      <a class="btn" href="https://www.linkedin.com/in/daniel-patterson-b03a5718b">LinkedIn</a>
      <a class="btn" href="mailto:dpatterson6575@gmail.com">Email</a>
      <a class="btn" href="https://github.com/danielpatterson1">GitHub</a>
      <a class="btn" href="./">Portfolio</a>
    </div>
    <p class="fine">Based in Tampa, Florida.<br>
    Employment work is summarized without proprietary figures. Independent projects use public datasets.</p>
  </div>
</footer>

</body>
</html>
