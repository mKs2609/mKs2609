<h1 align="center">Mohit Kumar</h1>

<p align="center">
  <b>I build AI systems that show their work.</b><br>
  RAG platforms · ML forecasting · full-stack products, tested and deployed
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/mohitkumar55gg/"><img src="https://img.shields.io/badge/LinkedIn-Mohit%20Kumar-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:mohitks2609@gmail.com"><img src="https://img.shields.io/badge/Email-mohitks2609%40gmail.com-555555?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/Open%20to-2027%20internships-2DA44E?style=flat-square" alt="Open to 2027 internships">
</p>

---

I'm a third-year B.Tech AI & Data Science student at VIPS-TC, New Delhi (GGSIPU, batch 2024–2028, CGPA 8.45).

I design, build and deploy AI applications end to end, from the database schema to the live URL. Every project below is a solo build with a live deployment, an automated test suite, and CI that runs on every push.

**Experience:** SDE Intern at **Zomakarb AI Solutions LLP**, New Delhi (Jul – Sep 2026). I designed and built a retrieval-augmented generation (RAG) assistant for the company, covering vector retrieval, document preprocessing pipelines and the generative AI application around them.

## Selected work

<table>
<tr>
<td width="44%" valign="top">
<a href="https://setu-ner-web.vercel.app"><img src="https://raw.githubusercontent.com/mKs2609/setu_ner/master/docs/images/map.jpg" alt="SetuNER map of road accessibility in Cachar, Assam"></a>
</td>
<td valign="top">
<h3>SetuNER</h3>
<b>Which roads in flood-prone Assam will still be passable tomorrow?</b>
<br><br>
A forecasting and relief-logistics system built on live government flood reports, satellite rainfall and terrain data.
<ul>
<li>Scores 110,000+ road segments, refreshed every morning by an automated pipeline</li>
<li>Onset AUC 0.71 on a held-out monsoon season, against 0.50 for the "same as today" baseline</li>
<li>Relief planner written as a linear program that reports which constraint is limiting: stock, trucks or reachability</li>
<li>316 API tests, 15 web tests, and outside-in alerting that emails me when a feed goes stale</li>
</ul>
<code>Python</code> <code>FastAPI</code> <code>PostGIS</code> <code>OR-Tools</code> <code>Next.js</code> <code>MapLibre</code> <code>Docker</code>
<br><br>
<a href="https://setu-ner-web.vercel.app"><b>Live app</b></a> · <a href="https://github.com/mKs2609/setu_ner"><b>Code</b></a> · <a href="https://github.com/mKs2609/setu_ner/actions/workflows/ci.yml"><img src="https://github.com/mKs2609/setu_ner/actions/workflows/ci.yml/badge.svg" alt="CI status"></a>
</td>
</tr>
<tr>
<td width="44%" valign="top">
<a href="https://rag-assistant-gamma.vercel.app"><img src="https://raw.githubusercontent.com/mKs2609/rag-assistant/main/docs/screenshots/chat.png" alt="RAG Assistant answering a question with a verified chart and citations"></a>
</td>
<td valign="top">
<h3>RAG Assistant</h3>
<b>Document Q&amp;A that still works when a second team logs in.</b>
<br><br>
A multi-tenant platform that answers questions from your own documents and checks every citation against its source.
<ul>
<li>Hybrid retrieval: pgvector similarity merged with Postgres full-text search</li>
<li>Workspace isolation enforced by Row-Level Security on every table and the storage bucket</li>
<li>Built-in evaluation harness that scores retrieval and answer accuracy across runs</li>
<li>One GIN index cut keyword search from 1,716 ms to 311 ms on 20,000 chunks</li>
</ul>
<code>TypeScript</code> <code>Next.js</code> <code>Supabase</code> <code>PostgreSQL</code> <code>pgvector</code> <code>Gemini</code> <code>Voyage AI</code>
<br><br>
<a href="https://rag-assistant-gamma.vercel.app"><b>Live demo</b></a> · <a href="https://github.com/mKs2609/rag-assistant"><b>Code</b></a> · <a href="https://github.com/mKs2609/rag-assistant/actions/workflows/ci.yml"><img src="https://github.com/mKs2609/rag-assistant/actions/workflows/ci.yml/badge.svg" alt="CI status"></a>
</td>
</tr>
<tr>
<td width="44%" valign="top">
<a href="https://burnout-buster-tp2wbhw5ctpsd3ggy8yzlc.streamlit.app/"><img src="https://raw.githubusercontent.com/mKs2609/burnout-buster/main/docs/screenshots/analytics.png" alt="Burnout Buster analytics dashboard for counselors"></a>
</td>
<td valign="top">
<h3>Burnout Buster</h3>
<b>An early warning for counselors, before a student has to ask for help.</b>
<br><br>
A three-minute wellness check-in for students and a risk dashboard for the counselors who support them.
<ul>
<li>Monotonic gradient-boosting models: more sleep or more support can never raise a risk score</li>
<li>Every score is explained by the answers that pushed it up or down</li>
<li>About 83% accuracy on 1,000 held-out students (the training data is simulated, and the app says so)</li>
<li>74 tests covering the model's guarantees, storage and UI flows</li>
</ul>
<code>Python</code> <code>scikit-learn</code> <code>Streamlit</code> <code>SQLAlchemy</code> <code>PostgreSQL</code> <code>Plotly</code>
<br><br>
<a href="https://burnout-buster-tp2wbhw5ctpsd3ggy8yzlc.streamlit.app/"><b>Live demo</b></a> · <a href="https://github.com/mKs2609/burnout-buster"><b>Code</b></a> · <a href="https://github.com/mKs2609/burnout-buster/actions/workflows/tests.yml"><img src="https://github.com/mKs2609/burnout-buster/actions/workflows/tests.yml/badge.svg" alt="Tests status"></a>
</td>
</tr>
</table>

## How I work

**I measure before I optimise.** Sending scanned pages to OCR in parallel looked like the obvious speed-up. Measured on a 23-page scan, it took 252 seconds against 34 seconds one batch at a time, so the pipeline runs sequentially. [Engineering decisions in RAG Assistant →](https://github.com/mKs2609/rag-assistant#engineering-decisions)

**I publish the results that don't flatter me.** SetuNER grades every forecast against a baseline once the outcome is known, and its live track record is on the forecast page, including the stretch where it lost. [Results, stated honestly →](https://github.com/mKs2609/setu_ner#results-stated-honestly)

**I write down why.** SetuNER has 18 numbered decision records, including the ones that record a failure, so the reasoning behind the system outlives my memory of it. [Decision records →](https://github.com/mKs2609/setu_ner/tree/master/docs/decisions)

**I make the system fail safely.** Burnout Buster refuses to save a model that fails any of its 8 sanity checks. SetuNER serves the baseline whenever the model loses to it.

## Toolbox

| | |
|---|---|
| **Languages** | Python, TypeScript, JavaScript, Java, C, SQL |
| **Backend** | FastAPI, Spring Boot, Flask, Next.js API routes, REST |
| **Frontend** | React, Next.js, Tailwind CSS, Streamlit |
| **AI and data** | RAG, embeddings, LLM APIs (Gemini, Voyage AI), scikit-learn, Pandas, NumPy, OR-Tools |
| **Databases** | PostgreSQL, pgvector, PostGIS, Supabase, SQLite |
| **Testing and delivery** | pytest, Vitest, Playwright, GitHub Actions, Docker, Vercel, Render |
| **AI-assisted development** | Claude Code |

## Right now

- **Building [Casewright](https://github.com/mKs2609/casewright):** an AI security analyst that investigates incidents with tools, builds an evidence chain, and waits for a human before any risky action. Java + Spring Boot gateway done (Argon2 auth, rotating JWT refresh tokens, CI); the Python agent is next
- **Looking for** a software engineering or AI engineering internship in 2027: [mohitks2609@gmail.com](mailto:mohitks2609@gmail.com)

<sub>Certifications: IBM SkillsBuild ([Build an AI Agent](https://www.credly.com/go/qDTQDkTv), [Craft Precise Prompts](https://www.credly.com/go/xZLCrnDe)) · Anthropic [Claude 101](https://github.com/mKs2609/mKs2609/blob/main/certificates/certificate-anthropic.pdf) · Forage job simulations ([Deloitte Cyber Security](https://github.com/mKs2609/mKs2609/blob/main/certificates/Cyber_job_Deloitte_certificate.pdf), [Tata GenAI Data Analytics](https://github.com/mKs2609/mKs2609/blob/main/certificates/genai_tata_jobsimulation_certificate.pdf))</sub>