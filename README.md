<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>James Andersen — Portfolio</title>
<style>
  :root{
    --bg:#EFEEE8;
    --bg-deep:#181A17;
    --ink:#1C1E1B;
    --ink-soft:#63655D;
    --ink-faint:#9A9C93;
    --line:#D7D5CA;
    --line-deep:#34372F;
    --green:#3E5F4C;
    --green-dim:#8FA396;
    --green-tint:#DEE6DF;
    --coral:#B15A41;
    --coral-tint:#EAD0C4;
    --card:#F8F7F2;
    --white:#F3F2EC;
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html,body{background:#444;}
  body{font-family:'Inter',sans-serif;color:var(--ink);}
  .page{
    width:1600px;height:1000px;position:relative;background:var(--bg);
    padding:60px 88px 56px;overflow:hidden;page-break-after:always;
  }
  .page:last-of-type{page-break-after:avoid;}
  .page.dark{background:var(--bg-deep);color:var(--white);}

  /* ---- typography ---- */
  h1,h2,h3{font-family:'Space Grotesk',sans-serif;font-weight:600;color:inherit;}
  .display{font-family:'Space Grotesk',sans-serif;}
  .mono{font-family:'IBM Plex Mono',monospace;}
  .eyebrow{
    font-family:'IBM Plex Mono',monospace;font-size:12.5px;letter-spacing:.16em;
    text-transform:uppercase;color:var(--coral);display:flex;align-items:center;gap:10px;margin-bottom:20px;
  }
  .eyebrow .idx{
    width:22px;height:22px;border:1px solid var(--coral);border-radius:2px;display:flex;
    align-items:center;justify-content:center;font-size:10.5px;color:var(--coral);
  }
  .page.dark .eyebrow{color:var(--green-dim);}
  .page.dark .eyebrow .idx{border-color:var(--green-dim);color:var(--green-dim);}
  .h1{font-size:52px;line-height:1.06;font-weight:600;letter-spacing:-.01em;}
  .h1 small{display:block;font-size:20px;font-weight:400;color:var(--ink-soft);margin-top:10px;letter-spacing:0;font-family:'Inter',sans-serif;}
  .kicker{font-size:15px;color:var(--ink-soft);max-width:640px;line-height:1.6;margin-top:18px;}
  .rule{height:1px;background:var(--line);width:100%;margin:28px 0;}
  .page.dark .rule{background:var(--line-deep);}

  /* ---- footer / corner ticks ---- */
  .foot{
    position:absolute;left:88px;right:88px;bottom:40px;display:flex;justify-content:space-between;
    font-family:'IBM Plex Mono',monospace;font-size:10.5px;letter-spacing:.1em;color:var(--ink-faint);
    border-top:1px solid var(--line);padding-top:14px;text-transform:uppercase;
  }
  .page.dark .foot{color:#7C7F76;border-top-color:var(--line-deep);}
  .tick{position:absolute;font-family:'IBM Plex Mono',monospace;font-size:10px;color:var(--ink-faint);letter-spacing:.08em;}
  .tick.tl{top:36px;left:88px;} .tick.tr{top:36px;right:88px;}
  .page.dark .tick{color:#6E7169;}

  /* ---- large index watermark : fills quiet lower-right space, echoes the page numbering system ---- */
  .pagenum{
    position:absolute;right:60px;bottom:56px;font-family:'Space Grotesk',sans-serif;font-weight:600;
    font-size:300px;line-height:1;color:var(--ink);opacity:.045;pointer-events:none;letter-spacing:-.02em;
  }

  /* ---- grid / cards ---- */
  .grid3{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;}
  .grid2{display:grid;grid-template-columns:1fr 1fr;gap:24px;}
  .card{background:var(--card);border:1px solid var(--line);border-radius:3px;padding:26px 26px;}
  .page.dark .card{background:#1F221E;border-color:var(--line-deep);}
  .tag{
    font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.04em;color:var(--ink-soft);
    border:1px solid var(--line);padding:5px 10px;border-radius:2px;display:inline-block;margin:0 6px 6px 0;background:var(--bg);
  }
  .tag.on{border-color:var(--green);color:var(--green);}

  /* ---- metric block ---- */
  .metric-num{font-family:'Space Grotesk',sans-serif;font-weight:600;font-size:46px;line-height:1;color:var(--green);}
  .metric-num.coral{color:var(--coral);}
  .metric-lab{font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.1em;color:var(--ink-soft);text-transform:uppercase;margin-top:8px;}

  svg text{font-family:'IBM Plex Mono',monospace;}
</style>
</head>
<body>

<!-- ============================================================ PAGE 01 — COVER ============================================================ -->
<section class="page dark">
  <div class="tick tl">JA / PORTFOLIO</div>
  <div class="tick tr">2026</div>

  <svg style="position:absolute;inset:0;opacity:.5" width="1600" height="1000" viewBox="0 0 1600 1000">
    <g stroke="#2B2E27" stroke-width="1">
      <line x1="0" y1="250" x2="1600" y2="250"/>
      <line x1="0" y1="500" x2="1600" y2="500"/>
      <line x1="0" y1="750" x2="1600" y2="750"/>
      <line x1="400" y1="0" x2="400" y2="1000"/>
      <line x1="800" y1="0" x2="800" y2="1000"/>
      <line x1="1200" y1="0" x2="1200" y2="1000"/>
    </g>
    <polyline points="120,860 340,790 560,820 780,690 1000,720 1220,560 1440,600" fill="none" stroke="#3E5F4C" stroke-width="2" opacity=".55"/>
    <g fill="#B15A41" opacity=".8">
      <circle cx="120" cy="860" r="4"/><circle cx="340" cy="790" r="4"/><circle cx="560" cy="820" r="4"/>
      <circle cx="780" cy="690" r="4"/><circle cx="1000" cy="720" r="4"/><circle cx="1220" cy="560" r="4"/><circle cx="1440" cy="600" r="4"/>
    </g>
  </svg>

  <div style="position:relative;height:100%;display:flex;flex-direction:column;justify-content:center;max-width:1100px;">
    <div class="mono" style="font-size:12.5px;letter-spacing:.2em;color:#8FA396;text-transform:uppercase;margin-bottom:26px;">Portfolio — 2026</div>
    <h1 class="display" style="font-size:104px;font-weight:600;line-height:0.98;letter-spacing:-.02em;color:var(--white);">JAMES<br>ANDERSEN</h1>
    <div style="margin-top:34px;display:flex;align-items:center;gap:16px;">
      <div style="font-size:22px;color:#D8D6CD;font-family:'Inter',sans-serif;">Data Analyst &amp; BI</div>
    </div>
    <div class="mono" style="margin-top:14px;font-size:14.5px;letter-spacing:.06em;color:#8FA396;">
      SQL <span style="color:#5B5E56">/</span> PYTHON <span style="color:#5B5E56">/</span> SPARK <span style="color:#5B5E56">/</span> POWER BI <span style="color:#5B5E56">/</span> POSTGRESQL
    </div>
    <div class="mono" style="margin-top:10px;font-size:12px;letter-spacing:.06em;color:#6E7169;">
      Information Systems, Multimedia Nusantara University — Class of 2026
    </div>
  </div>

  <div class="foot" style="color:#8B8E84;border-top-color:#2B2E27;">
    <span>jamesandersen112@gmail.com</span>
    <span>linkedin.com/in/james-andersen-06261a270</span>
    <span>github.com/jmsand12</span>
  </div>
</section>

<!-- ============================================================ PAGE 02 — ABOUT ============================================================ -->
<section class="page">
  <div class="pagenum">02</div>
  <div class="eyebrow"><span class="idx">01</span> Profile</div>
  <h1 class="h1">About Me</h1>

  <div style="display:flex;gap:64px;margin-top:36px;">
    <p style="max-width:640px;font-size:17px;line-height:1.75;color:var(--ink);">
      I build the pipelines, models, and dashboards that turn raw transactional and operational data into
      decisions. Working across <strong>SQL</strong>, <strong>Python</strong>, <strong>Power BI</strong>, and
      <strong>Apache Spark</strong>, my project work spans a 7.48M-row distributed fraud-detection pipeline,
      two shipped BI dashboards, and a production-style RAG application — end to end, from raw data to
      an interface a decision-maker can actually use. I'm finishing a B.S. in Information Systems at
      Multimedia Nusantara University (2026) with that work as the throughline.
    </p>
    <div style="width:1px;background:var(--line);"></div>
    <div class="mono" style="font-size:12px;color:var(--ink-soft);line-height:2.1;padding-top:4px;">
      LOCATION<br><span style="color:var(--ink)">Tangerang, ID</span><br><br>
      EDUCATION<br><span style="color:var(--ink)">UMN — Info. Systems, '26</span><br><br>
      TARGETING<br><span style="color:var(--ink)">Data Analyst / BI / Data Eng.</span>
    </div>
  </div>

  <div class="rule"></div>

  <div class="grid3">
    <div class="card">
      <div class="metric-num">7.48M+</div>
      <div class="metric-lab" style="margin-top:8px;">Rows Processed — FraudShield</div>
    </div>
    <div class="card">
      <div class="metric-num coral">0.993</div>
      <div class="metric-lab" style="margin-top:8px;">ROC-AUC, Fraud Classifier</div>
    </div>
    <div class="card">
      <div class="metric-num">3</div>
      <div class="metric-lab" style="margin-top:8px;">Dashboards Shipped — Power BI / Tableau</div>
    </div>
  </div>

  <div class="rule"></div>

  <div class="grid3">
    <div class="card">
      <div class="metric-lab" style="color:var(--green);margin-bottom:12px;">Data Analytics</div>
      <div style="font-size:15px;color:var(--ink-soft);line-height:1.6;">Python · SQL · Pandas · Data Visualization</div>
    </div>
    <div class="card">
      <div class="metric-lab" style="color:var(--green);margin-bottom:12px;">Business Intelligence</div>
      <div style="font-size:15px;color:var(--ink-soft);line-height:1.6;">Power BI · Tableau · DAX · Power Query</div>
    </div>
    <div class="card">
      <div class="metric-lab" style="color:var(--green);margin-bottom:12px;">Big Data &amp; ML</div>
      <div style="font-size:15px;color:var(--ink-soft);line-height:1.6;">Apache Spark · PySpark · GBT · SHAP</div>
    </div>
  </div>

  <div class="foot"><span>James Andersen</span><span>Profile</span><span>02 / 14</span></div>
</section>

<!-- ============================================================ PAGE 03 — EXPERIENCE ============================================================ -->
<section class="page">
  <div class="pagenum">03</div>
  <div class="eyebrow"><span class="idx">02</span> Experience</div>
  <h1 class="h1">Experience</h1>

  <div style="margin-top:44px;">
    <div style="display:flex;gap:40px;">
      <div class="mono" style="font-size:13px;color:var(--coral);width:40px;padding-top:6px;">01</div>
      <div style="flex:1;">
        <div style="display:flex;justify-content:space-between;align-items:baseline;">
          <h3 style="font-size:24px;">Web Developer</h3>
          <div class="mono" style="font-size:12px;color:var(--ink-soft);">AUG 2025 — DEC 2025</div>
        </div>
        <div style="font-size:14px;color:var(--ink-soft);margin-top:4px;">UMN Student Development</div>
        <ul style="margin-top:16px;padding-left:18px;font-size:15px;line-height:1.9;color:var(--ink);max-width:960px;">
          <li>Built and shipped an internal ticketing system (PHP, PDO, MySQL, JavaScript, Chart.js) that replaced ad-hoc, untracked coordination with a centralized workflow for Student Engagement.</li>
          <li>Designed the KPI and trend dashboard layer with Chart.js, giving staff a live view of ticket volume and status rather than manual spreadsheet tracking.</li>
          <li>Owned the project across the full SDLC — planning, analysis, design, implementation, testing, and deployment.</li>
          <li>Wrote and ran black-box test cases to validate core workflows before handoff.</li>
        </ul>
        <div style="margin-top:14px;">
          <span class="tag on">PHP</span><span class="tag on">MySQL</span><span class="tag on">JavaScript</span><span class="tag on">Chart.js</span><span class="tag on">SDLC</span>
        </div>
      </div>
    </div>

    <div class="rule" style="margin:36px 0;"></div>

    <div style="display:flex;gap:40px;align-items:baseline;">
      <div class="mono" style="font-size:13px;color:var(--ink-soft);width:40px;">02</div>
      <div style="flex:1;display:flex;justify-content:space-between;align-items:baseline;">
        <div>
          <span style="font-size:15px;color:var(--ink-soft);">Public Relations, KPU UMN</span>
          <span style="font-size:13.5px;color:var(--ink-faint);"> — analyzed social media trends to inform content strategy and cross-functional recommendations.</span>
        </div>
        <div class="mono" style="font-size:12px;color:var(--ink-faint);white-space:nowrap;margin-left:24px;">APR — DEC 2023</div>
      </div>
    </div>
  </div>

  <div class="foot"><span>James Andersen</span><span>Experience</span><span>03 / 14</span></div>
</section>

<!-- ============================================================ PAGE 04 — TECHNICAL SKILLS ============================================================ -->
<section class="page">
  <div class="pagenum">04</div>
  <div class="eyebrow"><span class="idx">03</span> Skills</div>
  <h1 class="h1">Technical Skills</h1>

  <div class="grid3" style="margin-top:40px;">
    <div class="card">
      <div class="metric-lab" style="color:var(--coral);">Data Analytics</div>
      <div class="rule" style="margin:14px 0;"></div>
      <div>
        <span class="tag">Python</span><span class="tag">Pandas</span><span class="tag">NumPy</span>
        <span class="tag">Matplotlib</span><span class="tag">Statistics</span><span class="tag">SQL</span>
      </div>
    </div>
    <div class="card">
      <div class="metric-lab" style="color:var(--coral);">Business Intelligence</div>
      <div class="rule" style="margin:14px 0;"></div>
      <div>
        <span class="tag">Power BI</span><span class="tag">DAX</span><span class="tag">Power Query</span><span class="tag">Tableau</span>
      </div>
    </div>
    <div class="card">
      <div class="metric-lab" style="color:var(--coral);">Database &amp; Big Data</div>
      <div class="rule" style="margin:14px 0;"></div>
      <div>
        <span class="tag">PostgreSQL</span><span class="tag">MySQL</span><span class="tag">Apache Spark</span>
        <span class="tag">PySpark</span><span class="tag">Spark SQL</span><span class="tag">JDBC</span>
      </div>
    </div>
  </div>

  <div class="grid2" style="margin-top:24px;">
    <div class="card">
      <div class="metric-lab" style="color:var(--coral);">Machine Learning / AI</div>
      <div class="rule" style="margin:14px 0;"></div>
      <div>
        <span class="tag">Scikit-learn</span><span class="tag">Spark ML</span><span class="tag">SHAP</span>
        <span class="tag">RAG</span><span class="tag">LLaMA 3.1</span><span class="tag">Sentence Transformers</span>
      </div>
    </div>
    <div class="card">
      <div class="metric-lab" style="color:var(--coral);">Development</div>
      <div class="rule" style="margin:14px 0;"></div>
      <div>
        <span class="tag">PHP</span><span class="tag">JavaScript</span><span class="tag">Figma</span>
        <span class="tag">Git</span><span class="tag">XAMPP</span><span class="tag">Jupyter</span><span class="tag">VS Code</span>
      </div>
    </div>
  </div>

  <div class="foot"><span>James Andersen</span><span>Technical Skills</span><span>04 / 14</span></div>
</section>

<!-- ============================================================ PAGE 05 — FEATURED PROJECT INTRO ============================================================ -->
<section class="page dark">
  <div class="tick tl mono" style="color:#7C7F76;">SELECTED WORK / 01</div>
  <div class="tick tr mono" style="color:#7C7F76;">FRAUD DETECTION</div>

  <div style="margin-top:70px;">
    <div class="eyebrow" style="color:var(--coral);"><span class="idx" style="border-color:var(--coral);color:var(--coral);">01</span> Featured Project</div>
    <h1 class="display" style="font-size:88px;color:var(--white);font-weight:600;letter-spacing:-.01em;">FraudShield</h1>
    <div style="font-size:19px;color:#B7BAB1;margin-top:12px;max-width:760px;">Large-Scale Digital Transaction Fraud Detection</div>
  </div>

  <div class="grid3" style="margin-top:56px;">
    <div style="grid-column:span 3;">
      <div class="metric-num" style="color:var(--coral);font-size:64px;">7.48M+</div>
      <div class="metric-lab" style="color:#9A9C93;">Transactions Processed</div>
    </div>
  </div>

  <div class="rule" style="background:#2E312A;margin:36px 0;"></div>

  <div class="grid3">
    <div>
      <div style="font-size:16px;color:var(--white);font-family:'Space Grotesk',sans-serif;">Apache Spark</div>
      <div style="font-size:13px;color:#8B8E84;margin-top:6px;">Large-scale distributed processing</div>
    </div>
    <div>
      <div style="font-size:16px;color:var(--white);font-family:'Space Grotesk',sans-serif;">Gradient Boosted Tree</div>
      <div style="font-size:13px;color:#8B8E84;margin-top:6px;">Fraud classification model</div>
    </div>
    <div>
      <div style="font-size:16px;color:var(--white);font-family:'Space Grotesk',sans-serif;">SHAP</div>
      <div style="font-size:13px;color:#8B8E84;margin-top:6px;">Explainable AI</div>
    </div>
    <div>
      <div style="font-size:16px;color:var(--white);font-family:'Space Grotesk',sans-serif;">PostgreSQL</div>
      <div style="font-size:13px;color:#8B8E84;margin-top:6px;">Source data storage</div>
    </div>
  </div>

  <p style="max-width:760px;font-size:14.5px;line-height:1.75;color:#9A9C93;margin-top:44px;">
    A large-scale fraud detection workflow built with Apache Spark and PySpark on a transaction dataset
    of approximately 7.48 million rows — covering data ingestion, preprocessing, feature engineering,
    model training, evaluation, and explainability.
  </p>

  <div class="foot" style="color:#7C7F76;border-top-color:#2B2E27;"><span>James Andersen</span><span>FraudShield</span><span>05 / 14</span></div>
</section>

<!-- ============================================================ PAGE 06 — FRAUDSHIELD ARCHITECTURE ============================================================ -->
<section class="page">
  <div class="eyebrow"><span class="idx">01</span> FraudShield — Pipeline</div>
  <h1 class="h1" style="font-size:42px;">Data Pipeline &amp; Architecture</h1>

  <div style="margin-top:44px;">
    <svg width="1424" height="540" viewBox="0 0 1424 540">
      <defs>
        <marker id="arrow" markerWidth="8" markerHeight="8" refX="6" refY="3" orient="auto">
          <path d="M0,0 L6,3 L0,6 Z" fill="#63655D"/>
        </marker>
      </defs>
      <!-- stage boxes: two rows of 5 -->
      <!-- row 1 -->
      <g font-family="IBM Plex Mono" font-size="13" fill="#1C1E1B">
        <!-- Box template function replicated manually -->
        <g>
          <rect x="0" y="0" width="250" height="92" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/>
          <text x="20" y="30" fill="#B15A41" font-size="11">01</text>
          <text x="20" y="56" font-family="Space Grotesk" font-size="17" fill="#1C1E1B">PostgreSQL</text>
          <text x="20" y="78" fill="#63655D" font-size="11.5">Source transactions</text>
        </g>
        <g transform="translate(293,0)">
          <rect width="250" height="92" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/>
          <text x="20" y="30" fill="#B15A41" font-size="11">02</text>
          <text x="20" y="56" font-family="Space Grotesk" font-size="17">JDBC</text>
          <text x="20" y="78" fill="#63655D" font-size="11.5">Connection layer</text>
        </g>
        <g transform="translate(586,0)">
          <rect width="250" height="92" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/>
          <text x="20" y="30" fill="#B15A41" font-size="11">03</text>
          <text x="20" y="56" font-family="Space Grotesk" font-size="17">PySpark DataFrame</text>
          <text x="20" y="78" fill="#63655D" font-size="11.5">Distributed loading</text>
        </g>
        <g transform="translate(879,0)">
          <rect width="250" height="92" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/>
          <text x="20" y="30" fill="#B15A41" font-size="11">04</text>
          <text x="20" y="56" font-family="Space Grotesk" font-size="17">Data Cleaning</text>
          <text x="20" y="78" fill="#63655D" font-size="11.5">Nulls · JSON parsing</text>
        </g>
        <g transform="translate(1172,0)">
          <rect width="252" height="92" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/>
          <text x="20" y="30" fill="#B15A41" font-size="11">05</text>
          <text x="20" y="56" font-family="Space Grotesk" font-size="17">Spark SQL</text>
          <text x="20" y="78" fill="#63655D" font-size="11.5">Structured querying</text>
        </g>
      </g>

      <!-- connecting arrows row1 left-to-right -->
      <g stroke="#63655D" stroke-width="1.4" marker-end="url(#arrow)">
        <line x1="250" y1="46" x2="291" y2="46"/>
        <line x1="543" y1="46" x2="584" y2="46"/>
        <line x1="836" y1="46" x2="877" y2="46"/>
        <line x1="1129" y1="46" x2="1170" y2="46"/>
      </g>
      <!-- drop down from row1 end to row2 start -->
      <path d="M1298,92 L1298,150 L1298,150" stroke="#63655D" stroke-width="1.4" fill="none" marker-end="url(#arrow)"/>

      <!-- row 2 : reversed direction, right to left -->
      <g transform="translate(0,220)" font-family="IBM Plex Mono" font-size="13" fill="#1C1E1B">
        <g transform="translate(1172,0)">
          <rect width="252" height="92" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/>
          <text x="20" y="30" fill="#3E5F4C" font-size="11">06</text>
          <text x="20" y="56" font-family="Space Grotesk" font-size="17">Feature Engineering</text>
          <text x="20" y="78" fill="#63655D" font-size="11.5">Derived variables</text>
        </g>
        <g transform="translate(879,0)">
          <rect width="250" height="92" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/>
          <text x="20" y="30" fill="#3E5F4C" font-size="11">07</text>
          <text x="20" y="56" font-family="Space Grotesk" font-size="17">Feature Encoding</text>
          <text x="20" y="78" fill="#63655D" font-size="11.5">Categorical → numeric</text>
        </g>
        <g transform="translate(586,0)">
          <rect width="250" height="92" rx="3" fill="#DEE6DF" stroke="#3E5F4C"/>
          <text x="20" y="30" fill="#3E5F4C" font-size="11">08</text>
          <text x="20" y="56" font-family="Space Grotesk" font-size="17">Gradient Boosted Tree</text>
          <text x="20" y="78" fill="#3E5F4C" font-size="11.5">Model training</text>
        </g>
        <g transform="translate(293,0)">
          <rect width="250" height="92" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/>
          <text x="20" y="30" fill="#3E5F4C" font-size="11">09</text>
          <text x="20" y="56" font-family="Space Grotesk" font-size="17">Fraud Prediction</text>
          <text x="20" y="78" fill="#63655D" font-size="11.5">Classification output</text>
        </g>
        <g transform="translate(0,0)">
          <rect width="250" height="92" rx="3" fill="#F3E4DC" stroke="#B15A41"/>
          <text x="20" y="30" fill="#B15A41" font-size="11">10</text>
          <text x="20" y="56" font-family="Space Grotesk" font-size="17">SHAP</text>
          <text x="20" y="78" fill="#B15A41" font-size="11.5">Explainability</text>
        </g>
      </g>
      <g stroke="#63655D" stroke-width="1.4" marker-end="url(#arrow)">
        <line x1="1172" y1="266" x2="1131" y2="266"/>
        <line x1="879" y1="266" x2="838" y2="266"/>
        <line x1="586" y1="266" x2="545" y2="266"/>
        <line x1="293" y1="266" x2="252" y2="266"/>
      </g>

      <!-- captions row -->
      <g font-family="IBM Plex Mono" font-size="12" fill="#63655D">
        <text x="0" y="400">Ingestion</text>
        <text x="293" y="400">Connectivity</text>
        <text x="586" y="400">Loading</text>
        <text x="879" y="400">Cleaning &amp; parsing</text>
        <text x="1172" y="400">Querying</text>
      </g>
      <g font-family="IBM Plex Mono" font-size="12" fill="#63655D">
        <text x="0" y="440">Explainability</text>
        <text x="293" y="440">Prediction</text>
        <text x="586" y="440">Training</text>
        <text x="879" y="440">Encoding</text>
        <text x="1172" y="440">Feature engineering</text>
      </g>
    </svg>
  </div>

  <p style="max-width:1100px;font-size:13.5px;color:var(--ink-soft);line-height:1.7;margin-top:8px;">
    Transactions are read from PostgreSQL via JDBC into a PySpark DataFrame, cleaned and parsed
    (including nested JSON fields), then queried with Spark SQL. Engineered features are encoded and
    passed to a Gradient Boosted Tree classifier; predictions are explained per-transaction using SHAP.
  </p>

  <div class="foot"><span>James Andersen</span><span>FraudShield — Architecture</span><span>06 / 14</span></div>
</section>

<!-- ============================================================ PAGE 07 — FRAUDSHIELD RESULTS ============================================================ -->
<section class="page">
  <div class="eyebrow"><span class="idx">01</span> FraudShield — Results</div>
  <h1 class="h1" style="font-size:42px;">Model Results</h1>

  <div class="grid3" style="margin-top:8px;">
    <div>
      <div class="metric-num">0.9930</div>
      <div class="metric-lab">ROC-AUC</div>
    </div>
    <div>
      <div class="metric-num coral">0.9629</div>
      <div class="metric-lab">F1-Score</div>
    </div>
    <div>
      <div class="metric-num">17,379</div>
      <div class="metric-lab">Rows / sec inference</div>
    </div>
  </div>
  <div class="mono" style="font-size:12px;color:var(--ink-faint);margin-top:10px;">DATASET — 7,483,766 rows · MODEL — Gradient Boosted Tree · TUNED &amp; SAMPLING-COMPARED</div>

  <div class="rule"></div>

  <div style="display:flex;gap:40px;">
    <div style="flex:1.1;">
      <div class="metric-lab" style="color:var(--coral);margin-bottom:14px;">Feature Importance (SHAP)</div>
      <svg width="620" height="230" viewBox="0 0 620 230">
        <g font-family="IBM Plex Mono" font-size="12.5" fill="#1C1E1B">
          <text x="0" y="14">distance_from_home</text>
          <rect x="0" y="20" width="560" height="16" fill="#3E5F4C"/>
          <text x="0" y="52">amount</text>
          <rect x="0" y="58" width="460" height="16" fill="#3E5F4C" opacity=".85"/>
          <text x="0" y="90">channel</text>
          <rect x="0" y="96" width="360" height="16" fill="#3E5F4C" opacity=".7"/>
          <text x="0" y="128">transaction_hour</text>
          <rect x="0" y="134" width="270" height="16" fill="#3E5F4C" opacity=".55"/>
          <text x="0" y="166">currency</text>
          <rect x="0" y="172" width="190" height="16" fill="#3E5F4C" opacity=".4"/>
        </g>
      </svg>
    </div>
    <div style="width:1px;background:var(--line);"></div>
    <div style="flex:1;">
      <div class="metric-lab" style="color:var(--coral);margin-bottom:14px;">ROC Curve</div>
      <svg width="420" height="230" viewBox="0 0 420 230">
        <line x1="30" y1="10" x2="30" y2="200" stroke="#D7D5CA"/>
        <line x1="30" y1="200" x2="400" y2="200" stroke="#D7D5CA"/>
        <line x1="30" y1="200" x2="400" y2="10" stroke="#D7D5CA" stroke-dasharray="3,4"/>
        <path d="M30,200 C 80,60 180,15 400,10" fill="none" stroke="#B15A41" stroke-width="2.4"/>
        <text x="330" y="30" font-family="IBM Plex Mono" font-size="12" fill="#B15A41">AUC 0.993</text>
        <text x="10" y="215" font-family="IBM Plex Mono" font-size="10" fill="#9A9C93">0</text>
        <text x="395" y="215" font-family="IBM Plex Mono" font-size="10" fill="#9A9C93">1</text>
      </svg>
    </div>
  </div>

  <div class="rule"></div>

  <div class="card" style="max-width:1100px;">
    <div class="metric-lab" style="color:var(--green);margin-bottom:10px;">Why GBT?</div>
    <p style="font-size:13.5px;line-height:1.7;color:var(--ink-soft);">
      Gradient Boosted Trees suit tabular transaction data, capture nonlinear relationships between
      features, and expose feature importance for interpretability — with native integration into Spark ML
      for distributed training. SHAP is layered on top to explain individual predictions.
    </p>
  </div>

  <div class="foot"><span>James Andersen</span><span>FraudShield — Results</span><span>07 / 14</span></div>
</section>

<!-- ============================================================ PAGE 08 — BI PROJECT ============================================================ -->
<section class="page">
  <div class="pagenum">08</div>
  <div class="eyebrow"><span class="idx">02</span> Business Intelligence</div>
  <h1 class="h1" style="font-size:42px;">Student Performance Analysis</h1>
  <div style="margin-top:10px;">
    <span class="tag on">Power BI</span><span class="tag on">Python</span><span class="tag on">Data Visualization</span>
  </div>

  <div style="display:flex;gap:44px;margin-top:32px;">
    <div style="flex:1;">
      <div class="grid2">
        <div><div class="metric-lab" style="color:var(--coral);">Problem</div><p style="font-size:13.5px;color:var(--ink-soft);margin-top:8px;line-height:1.6;">Score distributions, academic preferences, and university capacities lived in separate raw files with no single view for education-sector decision-making.</p></div>
        <div><div class="metric-lab" style="color:var(--coral);">Objective</div><p style="font-size:13.5px;color:var(--ink-soft);margin-top:8px;line-height:1.6;">Build one dashboard that connects score distribution to program preference and capacity, so gaps between demand and available seats are visible at a glance.</p></div>
        <div><div class="metric-lab" style="color:var(--coral);">Approach</div><p style="font-size:13.5px;color:var(--ink-soft);margin-top:8px;line-height:1.6;">Cleaned and joined the source data in Python (Pandas), then modeled relationships and built linked report pages in Power BI.</p></div>
        <div><div class="metric-lab" style="color:var(--coral);">Key Insight</div><p style="font-size:13.5px;color:var(--ink-soft);margin-top:8px;line-height:1.6;">Cross-referencing score distribution against preference share surfaced where student demand and program capacity were misaligned — the specific gap the dashboard was built to make visible.</p></div>
      </div>
      <div class="rule"></div>
      <div class="metric-lab" style="color:var(--green);">Tools</div>
      <div style="margin-top:10px;"><span class="tag">Power BI</span><span class="tag">Python</span><span class="tag">Data Preprocessing</span></div>
    </div>

    <div style="flex:1;">
      <div class="card" style="height:100%;">
        <div class="metric-lab" style="color:var(--ink-soft);margin-bottom:16px;">Dashboard — Illustrative View</div>
        <svg width="100%" height="330" viewBox="0 0 560 330">
          <rect x="0" y="0" width="560" height="330" fill="#F3F2EC" stroke="#D7D5CA"/>
          <g font-family="IBM Plex Mono" font-size="10.5" fill="#63655D">
            <text x="16" y="22">SCORE DISTRIBUTION</text>
            <g fill="#3E5F4C">
              <rect x="16" y="70" width="26" height="60"/>
              <rect x="52" y="40" width="26" height="90"/>
              <rect x="88" y="20" width="26" height="110"/>
              <rect x="124" y="55" width="26" height="75"/>
              <rect x="160" y="90" width="26" height="40"/>
            </g>
            <text x="16" y="150">PREFERENCE SHARE</text>
            <circle cx="80" cy="215" r="46" fill="none" stroke="#B15A41" stroke-width="14" stroke-dasharray="180 300"/>
            <circle cx="80" cy="215" r="46" fill="none" stroke="#3E5F4C" stroke-width="14" stroke-dasharray="90 300" stroke-dashoffset="-180"/>
            <circle cx="80" cy="215" r="46" fill="none" stroke="#D7D5CA" stroke-width="14" stroke-dasharray="30 300" stroke-dashoffset="-270"/>
            <text x="230" y="150">CAPACITY BY REGION</text>
            <g stroke="#D7D5CA"><line x1="230" y1="170" x2="530" y2="170"/><line x1="230" y1="200" x2="530" y2="200"/><line x1="230" y1="230" x2="530" y2="230"/><line x1="230" y1="260" x2="530" y2="260"/></g>
            <polyline points="230,250 280,220 330,235 380,190 430,210 480,175 530,195" fill="none" stroke="#B15A41" stroke-width="2"/>
          </g>
        </svg>
      </div>
    </div>
  </div>

  <div class="foot"><span>James Andersen</span><span>Student Performance Analysis</span><span>08 / 14</span></div>
</section>

<!-- ============================================================ PAGE 09 — FLOOD DATA VIZ ============================================================ -->
<section class="page">
  <div class="pagenum">09</div>
  <div class="eyebrow"><span class="idx">03</span> Data Visualization</div>
  <h1 class="h1" style="font-size:42px;">Jakarta Flood Intensity Reports</h1>
  <div style="margin-top:10px;">
    <span class="tag on">Tableau</span><span class="tag on">Kaggle</span><span class="tag on">BNPB Data</span>
  </div>

  <div style="display:flex;gap:44px;margin-top:34px;">
    <div style="flex:1;">
      <div class="card" style="height:340px;">
        <div class="metric-lab" style="color:var(--ink-soft);margin-bottom:16px;">Regional Severity — Illustrative View</div>
        <svg width="100%" height="270" viewBox="0 0 560 270">
          <g>
            <rect x="20" y="20" width="120" height="90" fill="#F3E4DC" stroke="#B15A41"/>
            <rect x="150" y="20" width="120" height="90" fill="#DEE6DF" stroke="#3E5F4C"/>
            <rect x="280" y="20" width="120" height="90" fill="#F3E4DC" stroke="#B15A41" opacity=".7"/>
            <rect x="410" y="20" width="130" height="90" fill="#EFEEE8" stroke="#D7D5CA"/>
            <text x="30" y="55" font-family="IBM Plex Mono" font-size="11" fill="#B15A41">NORTH</text>
            <text x="30" y="72" font-family="IBM Plex Mono" font-size="9.5" fill="#8A5342">High priority</text>
            <text x="160" y="55" font-family="IBM Plex Mono" font-size="11" fill="#3E5F4C">EAST</text>
            <text x="290" y="55" font-family="IBM Plex Mono" font-size="11" fill="#B15A41">WEST</text>
            <text x="290" y="72" font-family="IBM Plex Mono" font-size="9.5" fill="#8A5342">High priority</text>
            <text x="420" y="55" font-family="IBM Plex Mono" font-size="11" fill="#63655D">SOUTH</text>

            <rect x="150" y="150" width="260" height="90" fill="#F3F2EC" stroke="#D7D5CA"/>
            <text x="160" y="175" font-family="IBM Plex Mono" font-size="11" fill="#63655D">CENTRAL</text>
          </g>
        </svg>
      </div>
    </div>
    <div style="flex:1;">
      <div style="display:flex;flex-direction:column;gap:22px;">
        <div><div class="metric-lab" style="color:var(--coral);">Problem</div><p style="font-size:13.5px;color:var(--ink-soft);margin-top:6px;line-height:1.6;">Flood frequency, severity, and impact varied widely across Jakarta's administrative regions without a unified view for planning.</p></div>
        <div><div class="metric-lab" style="color:var(--coral);">Approach</div><p style="font-size:13.5px;color:var(--ink-soft);margin-top:6px;line-height:1.6;">Combined BNPB and Kaggle datasets into an interactive Tableau dashboard analyzing flood frequency, severity, and regional impact.</p></div>
        <div><div class="metric-lab" style="color:var(--coral);">Key Insight</div><p style="font-size:13.5px;color:var(--ink-soft);margin-top:6px;line-height:1.6;">North and West Jakarta emerged as priority areas, informing discussion of flood mitigation and water catchment strategies.</p></div>
      </div>
    </div>
  </div>

  <div class="foot"><span>James Andersen</span><span>Jakarta Flood Intensity Reports</span><span>09 / 14</span></div>
</section>

<!-- ============================================================ PAGE 10 — TANYAVARA AI/RAG ============================================================ -->
<section class="page">
  <div class="eyebrow"><span class="idx">04</span> AI / Machine Learning</div>
  <h1 class="h1" style="font-size:42px;">TanyaVara</h1>
  <div class="kicker" style="margin-top:6px;">RAG-based university information chatbot — prototype project.</div>

  <div style="margin-top:16px;">
    <span class="tag on">LLaMA 3.1 8B</span><span class="tag on">RAG</span><span class="tag on">Sentence Transformers</span>
    <span class="tag on">BM25</span><span class="tag on">PyMuPDF</span><span class="tag on">MarianMT</span><span class="tag on">Streamlit</span>
  </div>

  <div style="margin-top:40px;">
    <svg width="1424" height="150" viewBox="0 0 1424 150">
      <defs>
        <marker id="arrow2" markerWidth="8" markerHeight="8" refX="6" refY="3" orient="auto">
          <path d="M0,0 L6,3 L0,6 Z" fill="#63655D"/>
        </marker>
      </defs>
      <g font-family="IBM Plex Mono" font-size="12.5" fill="#1C1E1B">
        <!-- 8 stages -->
        <g id="s0"><rect x="0" y="0" width="150" height="70" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/><text x="14" y="30" font-family="Space Grotesk" font-size="13">PDF Docs</text><text x="14" y="50" fill="#63655D" font-size="10">Source material</text></g>
        <g transform="translate(178,0)"><rect width="150" height="70" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/><text x="14" y="30" font-family="Space Grotesk" font-size="13">Extraction</text><text x="14" y="50" fill="#63655D" font-size="10">PyMuPDF</text></g>
        <g transform="translate(356,0)"><rect width="150" height="70" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/><text x="14" y="30" font-family="Space Grotesk" font-size="13">Preprocess</text><text x="14" y="50" fill="#63655D" font-size="10">Clean · translate</text></g>
        <g transform="translate(534,0)"><rect width="150" height="70" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/><text x="14" y="30" font-family="Space Grotesk" font-size="13">Chunking</text><text x="14" y="50" fill="#63655D" font-size="10">Segment text</text></g>
        <g transform="translate(712,0)"><rect width="150" height="70" rx="3" fill="#DEE6DF" stroke="#3E5F4C"/><text x="14" y="30" font-family="Space Grotesk" font-size="13" fill="#3E5F4C">Retrieval</text><text x="14" y="50" fill="#3E5F4C" font-size="10">BM25 + embeddings</text></g>
        <g transform="translate(890,0)"><rect width="150" height="70" rx="3" fill="#DEE6DF" stroke="#3E5F4C"/><text x="14" y="30" font-family="Space Grotesk" font-size="13" fill="#3E5F4C">LLaMA 3.1</text><text x="14" y="50" fill="#3E5F4C" font-size="10">Generation</text></g>
        <g transform="translate(1068,0)"><rect width="150" height="70" rx="3" fill="#F8F7F2" stroke="#D7D5CA"/><text x="14" y="30" font-family="Space Grotesk" font-size="13">Response</text><text x="14" y="50" fill="#63655D" font-size="10">MarianMT</text></g>
        <g transform="translate(1246,0)"><rect width="150" height="70" rx="3" fill="#F3E4DC" stroke="#B15A41"/><text x="14" y="30" font-family="Space Grotesk" font-size="13" fill="#B15A41">Streamlit</text><text x="14" y="50" fill="#B15A41" font-size="10">User interface</text></g>
      </g>
      <g stroke="#63655D" stroke-width="1.4" marker-end="url(#arrow2)">
        <line x1="150" y1="35" x2="176" y2="35"/><line x1="328" y1="35" x2="354" y2="35"/>
        <line x1="506" y1="35" x2="532" y2="35"/><line x1="684" y1="35" x2="710" y2="35"/>
        <line x1="862" y1="35" x2="888" y2="35"/><line x1="1040" y1="35" x2="1066" y2="35"/>
        <line x1="1218" y1="35" x2="1244" y2="35"/>
      </g>
    </svg>
  </div>

  <p style="max-width:1100px;font-size:14px;line-height:1.75;color:var(--ink-soft);margin-top:30px;">
    Built to answer university-related questions through a Retrieval-Augmented Generation approach: source
    PDFs are parsed and chunked, relevant passages are retrieved with a hybrid BM25 + embedding search,
    and LLaMA 3.1 8B generates grounded responses served through a Streamlit interface.
  </p>

  <div class="foot"><span>James Andersen</span><span>TanyaVara</span><span>10 / 14</span></div>
</section>

<!-- ============================================================ PAGE 11 — TICKETING SYSTEM ============================================================ -->
<section class="page">
  <div class="pagenum">11</div>
  <div class="eyebrow"><span class="idx">05</span> Web / Information Systems</div>
  <h1 class="h1" style="font-size:42px;">Internal Ticketing System</h1>
  <div style="margin-top:10px;">
    <span class="tag on">PHP</span><span class="tag on">PDO</span><span class="tag on">MySQL</span>
    <span class="tag on">JavaScript</span><span class="tag on">Chart.js</span><span class="tag on">XAMPP</span>
  </div>

  <div style="display:flex;gap:44px;margin-top:32px;">
    <div style="flex:1;">
      <div class="metric-lab" style="color:var(--coral);">Data Model</div>
      <p style="font-size:13.5px;color:var(--ink-soft);margin-top:8px;line-height:1.7;">
        A normalized MySQL schema tracks tickets through status states (open → pending → resolved),
        accessed through prepared PDO statements to keep the reporting layer consistent with the
        underlying data.
      </p>
      <div class="metric-lab" style="color:var(--coral);margin-top:22px;">Reporting Layer</div>
      <p style="font-size:13.5px;color:var(--ink-soft);margin-top:8px;line-height:1.7;">
        Chart.js components query that schema directly for status breakdowns and volume trends —
        the dashboard reads live from the same tables staff work in, not a static export.
      </p>
      <div class="metric-lab" style="color:var(--coral);margin-top:22px;">Full-Stack Ownership</div>
      <p style="font-size:13.5px;color:var(--ink-soft);margin-top:8px;line-height:1.7;">
        Worked across the full SDLC — schema design through deployment — with black-box test cases
        covering the core ticket workflow before handoff. (See Experience, p.03, for role context.)
      </p>
    </div>
    <div style="flex:1;">
      <div class="card" style="height:100%;">
        <div class="metric-lab" style="color:var(--ink-soft);margin-bottom:16px;">Dashboard — Illustrative View</div>
        <svg width="100%" height="330" viewBox="0 0 560 330">
          <rect x="0" y="0" width="560" height="330" fill="#F3F2EC" stroke="#D7D5CA"/>
          <g font-family="IBM Plex Mono" font-size="10.5" fill="#63655D">
            <rect x="16" y="16" width="120" height="60" fill="#DEE6DF" stroke="#3E5F4C"/>
            <text x="26" y="36">OPEN</text><circle cx="32" cy="52" r="5" fill="#3E5F4C"/><circle cx="48" cy="52" r="5" fill="#3E5F4C"/><circle cx="64" cy="52" r="5" fill="#3E5F4C"/>
            <rect x="150" y="16" width="120" height="60" fill="#F3E4DC" stroke="#B15A41"/>
            <text x="160" y="36">PENDING</text><circle cx="166" cy="52" r="5" fill="#B15A41"/><circle cx="182" cy="52" r="5" fill="#B15A41"/>
            <rect x="284" y="16" width="120" height="60" fill="#EFEEE8" stroke="#D7D5CA"/>
            <text x="294" y="36">RESOLVED</text><circle cx="300" cy="52" r="5" fill="#8A8C84"/><circle cx="316" cy="52" r="5" fill="#8A8C84"/><circle cx="332" cy="52" r="5" fill="#8A8C84"/><circle cx="348" cy="52" r="5" fill="#8A8C84"/>
            <text x="16" y="110">TICKET TREND</text>
            <g stroke="#D7D5CA"><line x1="16" y1="130" x2="540" y2="130"/><line x1="16" y1="160" x2="540" y2="160"/><line x1="16" y1="190" x2="540" y2="190"/></g>
            <polyline points="16,180 90,150 164,165 238,120 312,140 386,100 460,125 534,95" fill="none" stroke="#3E5F4C" stroke-width="2"/>
            <text x="16" y="230">TICKETS BY CATEGORY</text>
            <g fill="#B15A41"><rect x="16" y="250" width="60" height="16"/><rect x="16" y="270" width="100" height="16" opacity=".8"/><rect x="16" y="290" width="140" height="16" opacity=".6"/></g>
          </g>
        </svg>
      </div>
    </div>
  </div>

  <div class="foot"><span>James Andersen</span><span>Internal Ticketing System</span><span>11 / 14</span></div>
</section>

<!-- ============================================================ PAGE 12 — ADDITIONAL PROJECTS ============================================================ -->
<section class="page">
  <div class="pagenum">12</div>
  <div class="eyebrow"><span class="idx">06</span> More Work</div>
  <h1 class="h1" style="font-size:42px;">Additional Projects</h1>

  <div class="grid2" style="margin-top:40px;">
    <div class="card">
      <div class="metric-lab" style="color:var(--green);">Stroke Risk Classification Analysis</div>
      <div style="font-size:12px;color:var(--ink-faint);margin-top:6px;" class="mono">DATA ANALYTICS / ML</div>
      <p style="font-size:13.5px;color:var(--ink-soft);margin-top:14px;line-height:1.7;">
        Followed CRISP-DM end to end on a clinical risk dataset: handled missing values and outliers,
        trained a pruned decision tree, then read the resulting splits to identify which factors drove
        the model's risk predictions.
      </p>
      <div style="margin-top:14px;">
        <span class="tag">CRISP-DM</span><span class="tag">Decision Tree</span><span class="tag">Data Preprocessing</span>
      </div>
    </div>
    <div class="card">
      <div class="metric-lab" style="color:var(--green);">Supplies Request Website</div>
      <div style="font-size:12px;color:var(--ink-faint);margin-top:6px;" class="mono">WEB DEVELOPMENT</div>
      <p style="font-size:13.5px;color:var(--ink-soft);margin-top:14px;line-height:1.7;">
        Designed in Figma and built using the RAD methodology, with user feedback and UAT cycles shaping
        the final request-management workflow.
      </p>
      <div style="margin-top:14px;">
        <span class="tag">Figma</span><span class="tag">RAD</span><span class="tag">UAT</span>
      </div>
    </div>
  </div>

  <div class="foot"><span>James Andersen</span><span>Additional Projects</span><span>12 / 14</span></div>
</section>

<!-- ============================================================ PAGE 13 — EDUCATION ============================================================ -->
<section class="page">
  <div class="pagenum">13</div>
  <div class="eyebrow"><span class="idx">07</span> Background</div>
  <h1 class="h1" style="font-size:42px;">Education</h1>

  <div style="margin-top:48px;display:flex;gap:40px;">
    <div class="mono" style="font-size:13px;color:var(--coral);width:40px;padding-top:6px;">01</div>
    <div>
      <h3 style="font-size:22px;">Multimedia Nusantara University</h3>
      <div style="font-size:14px;color:var(--ink-soft);margin-top:6px;">Bachelor's Degree, Information Systems</div>
      <div class="mono" style="font-size:12px;color:var(--ink-faint);margin-top:6px;">2022 — 2026</div>
    </div>
  </div>

  <div class="rule" style="max-width:1100px;"></div>

  <p style="max-width:900px;font-size:13.5px;color:var(--ink-soft);line-height:1.7;">
    Coursework and independent projects centered on data analytics, business intelligence, database
    systems, and information-systems development — applied through the projects featured in this
    portfolio.
  </p>

  <div class="foot"><span>James Andersen</span><span>Education</span><span>13 / 14</span></div>
</section>

<!-- ============================================================ PAGE 14 — CONTACT ============================================================ -->
<section class="page dark">
  <svg style="position:absolute;inset:0;opacity:.5" width="1600" height="1000" viewBox="0 0 1600 1000">
    <g stroke="#2B2E27" stroke-width="1">
      <line x1="0" y1="250" x2="1600" y2="250"/><line x1="0" y1="500" x2="1600" y2="500"/><line x1="0" y1="750" x2="1600" y2="750"/>
      <line x1="400" y1="0" x2="400" y2="1000"/><line x1="800" y1="0" x2="800" y2="1000"/><line x1="1200" y1="0" x2="1200" y2="1000"/>
    </g>
  </svg>

  <div style="position:relative;height:100%;display:flex;flex-direction:column;justify-content:center;max-width:1000px;">
    <div class="mono" style="font-size:12.5px;letter-spacing:.2em;color:#8FA396;text-transform:uppercase;margin-bottom:26px;">14 / 14 — Contact</div>
    <h1 class="display" style="font-size:80px;font-weight:600;line-height:1.02;color:var(--white);">Let's Connect</h1>
    <div class="mono" style="font-size:14.5px;letter-spacing:.06em;color:#8FA396;margin-top:18px;">
      DATA ANALYTICS <span style="color:#5B5E56">/</span> BUSINESS INTELLIGENCE <span style="color:#5B5E56">/</span> BIG DATA
    </div>

    <div class="rule" style="background:#2E312A;max-width:600px;"></div>

    <div class="mono" style="font-size:15px;color:#D8D6CD;line-height:2.3;">
      EMAIL &nbsp; <span style="color:#F3F2EC">jamesandersen112@gmail.com</span><br>
      LINKEDIN &nbsp; <span style="color:#F3F2EC">linkedin.com/in/james-andersen-06261a270</span><br>
      GITHUB &nbsp; <span style="color:#F3F2EC">github.com/jmsand12</span><br>
      PHONE &nbsp; <span style="color:#F3F2EC">+62 851-7242-5514</span>
    </div>
  </div>

  <div class="foot" style="color:#8B8E84;border-top-color:#2B2E27;">
    <span>James Andersen</span><span>Information Systems — Data / BI / Big Data</span><span>2026</span>
  </div>
</section>

</body>
</html>
