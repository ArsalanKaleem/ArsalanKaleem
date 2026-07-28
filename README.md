<!--   ─────────────────────────────────────────────────────────────   HERO BANNER SUGGESTION   Replace the image below with a 1280x400 banner exported from   Figma / Canva. Recommended treatment:     • Background: #0D1117 → #161B22 vertical gradient     • Accent line: #00BFFF (matches typing SVG + badges)     • Left-aligned monospace text: "Arsalan Kaleem"       sub-line: "Flutter · Applied AI · Geospatial Systems"     • Right side: faint isometric grid or Sentinel-2 raster tile       at 12% opacity (ties into the GIS work)     • Export as banner.png → commit to /assets/banner.png   Subtle animation ideas (GIF, keep under 2 MB each):     • ForgeOS: repo-discovery feed scrolling, 6s loop     • TEMPUS: solver filling a timetable grid cell-by-cell     • SWAI: Sindh choropleth fading in by accessibility score   ───────────────────────────────────────────────────────────── --> <p align="center">   <img src="./assets/banner.png" alt="Arsalan Kaleem — Flutter, Applied AI, Geospatial Systems" width="100%" /> </p> <h2 align="center">Software Engineer — Flutter · Applied AI · Geospatial Systems</h2> <p align="center">   <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=22&pause=1200&color=00BFFF&center=true&vCenter=true&width=760&lines=Cross-platform+systems+across+6+targets;LLM+pipelines%2C+RAG%2C+and+agentic+workflows;Constraint+solvers+for+real+scheduling+problems;Geospatial+analytics+at+district+scale" alt="Typing SVG" /> </p> <p align="center">   <a href="https://arsalankaleem.github.io/portfolio/"><img src="https://img.shields.io/badge/Portfolio-0D1117?style=for-the-badge&logo=firefoxbrowser&logoColor=00BFFF" alt="Portfolio" /></a>   <a href="https://linkedin.com/in/arsalankaleem"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>   <a href="mailto:arsalanabbasi.here@gmail.com"><img src="https://img.shields.io/badge/Email-0D1117?style=for-the-badge&logo=gmail&logoColor=EA4335" alt="Email" /></a>   <img src="https://komarev.com/ghpvc/?username=ArsalanKaleem&style=for-the-badge&color=00BFFF&label=PROFILE+VIEWS" alt="Profile views" /> </p> <p align="center">   <img src="https://img.shields.io/badge/Based\_in-Pakistan-0D1117?style=flat-square&labelColor=161B22&color=00BFFF" alt="Location" />   <img src="https://img.shields.io/badge/Open\_to-Full--time\_·\_Remote\_·\_Contract-0D1117?style=flat-square&labelColor=161B22&color=00BFFF" alt="Availability" />   <img src="https://img.shields.io/badge/Focus-Flutter\_·\_AI\_·\_GIS-0D1117?style=flat-square&labelColor=161B22&color=00BFFF" alt="Focus" /> </p> ---

## ▍About

I build production-grade software where three disciplines intersect: **cross-platform application engineering**, **applied artificial intelligence**, and **geospatial analysis**.

My work spans a constraint-satisfaction scheduler that eliminates weeks of manual timetabling, a geospatial analytics platform that measures drinking-water accessibility for **5,159 villages** across Sindh, and an AI-assisted discovery tool that ships to **six platform targets** from a single Dart codebase.

The through-line is the same in each case — take an unglamorous, high-friction problem, model it correctly, and ship something people actually run.

**Engineering principles I hold to:**

* Architecture before features. Layered separation, immutable state, testable boundaries.
* Determinism at the core, intelligence at the edges. LLMs augment logic; they don't replace it.
* Offline-first by default. Network availability is a feature, not an assumption.
* Measure the impact or don't claim it.

**Domains:** Flutter · Artificial Intelligence · GIS & Remote Sensing · Backend Engineering · System Design · Developer Tools · Civic Technology · Open Source

---

## ▍What I'm Working On


| Project       | Focus                                                  | Status                                |
| :------------ | :----------------------------------------------------- | :------------------------------------ |
| **CivicPing** | Citizen-to-government issue reporting and routing      | Active development                    |
| **ForgeOS**   | AI-guided open source contribution discovery           | Iterating on the recommendation layer |
| **SWAI**      | Sindh Water Access Index — validation and publication | Research-phase writeup                |
| **RHAI**      | AI workflow automation and orchestration               | Architecture and prototyping          |

**Current technical focus:** multi-agent orchestration and tool-calling patterns, LangGraph, Model Context Protocol (MCP), containerized backend deployment, distributed system design.

---

## ▍Featured Projects

<!-- Repo pin cards render live from github-readme-stats.      Update the &repo= parameter if your repository slugs differ. --> ### ◆ ForgeOS — *Where you forge your open source career.*

**An AI-powered discovery platform that turns "I want to contribute to open source" into a concrete, ranked list of issues you can actually solve.**

Open source onboarding fails at the search step, not the coding step. ForgeOS aggregates trending repositories through the GitHub REST and GraphQL APIs, surfaces beginner-friendly issues filtered by language and difficulty, and layers Gemini-generated contribution guidance on top — repository context, codebase orientation, and a suggested approach for each issue.

Architecturally it is a Riverpod-driven, Freezed-modelled Flutter application with declarative GoRouter navigation, Dio-based API clients with request-level caching, and Hive for offline persistence so a browsing session survives connectivity loss.

**Impact:** collapses open source discovery from hours of manual GitHub filtering to a single ranked feed, and ships to **six targets** — Web, Android, Windows, macOS, Linux — from one codebase.

`Flutter``Riverpod``GoRouter``Dio``Hive``Freezed``GitHub REST API``GitHub GraphQL API``Gemini API`

<a href="https://github.com/ArsalanKaleem/ForgeOS">   <img src="https://github-readme-stats.vercel.app/api/pin/?username=ArsalanKaleem&repo=ForgeOS&theme=tokyonight&hide\_border=true&bg\_color=0D1117" alt="ForgeOS" /> </a> ---

### ◆ TEMPUS — *Automating university scheduling through intelligent optimization.*

**A Constraint Satisfaction Problem solver that generates conflict-free university timetables from institutional constraints.**

University timetabling is NP-hard and, in most institutions, still solved by hand across multiple weeks. TEMPUS models the problem formally — rooms, instructors, sections, capacities, and time slots as variables under hard and soft constraints — and applies constraint propagation with backtracking search to produce feasible schedules. Hard constraints (double-booked rooms, instructor collisions) are guaranteed; soft constraints (preferred slots, workload balance) are optimized.

Delivered as an administrator-facing Flutter application backed by Firebase, with Riverpod state management and Hive caching for offline schedule review.

**Impact:** reduced manual scheduling workload by **over 90%**, replacing a multi-week coordination cycle with a solver run measured in minutes.

`Flutter``Firebase``Riverpod``Hive``Constraint Satisfaction (CSP)`

<a href="https://github.com/ArsalanKaleem/TEMPUS">   <img src="https://github-readme-stats.vercel.app/api/pin/?username=ArsalanKaleem&repo=TEMPUS&theme=tokyonight&hide\_border=true&bg\_color=0D1117" alt="TEMPUS" /> </a> ---

### ◆ SWAI — Sindh Water Access Index — *Using geospatial intelligence to improve water accessibility.*

**A research-grade geospatial analytics platform quantifying drinking-water accessibility across 5,159 villages in Sindh, Pakistan.**

SWAI integrates Sentinel-2 imagery and Google Earth Engine collections with village-level administrative data to compute a composite accessibility score per settlement. The pipeline handles raster preprocessing and cloud masking in Earth Engine, spatial joins and distance-decay modelling in GeoPandas, and index normalization in Pandas and NumPy, with QGIS used for cartographic output.

Results are validated against official government datasets rather than presented in isolation — the methodology is reproducible and the outputs are publication-quality maps suitable for policy review.

**Impact:** produces village-level accessibility scores across **5,159 settlements**, validated against official datasets, directly supporting **UN SDG 6 (Clean Water and Sanitation)** measurement at district scale.

`Python``Google Earth Engine``Sentinel-2``QGIS``GeoPandas``Pandas``NumPy``Remote Sensing``Spatial Analysis`

<a href="https://github.com/ArsalanKaleem/SWAI">   <img src="https://github-readme-stats.vercel.app/api/pin/?username=ArsalanKaleem&repo=SWAI&theme=tokyonight&hide\_border=true&bg\_color=0D1117" alt="SWAI" /> </a> ---

### ◆ Aestimo — *An AI career copilot for the applicant tracking era.*

**End-to-end resume intelligence: parse, score against ATS criteria, rebuild, and prepare.**

Aestimo closes the loop between a candidate's raw experience and what automated screening systems actually reward. It analyzes uploaded resumes, scores them against ATS parsing and keyword criteria, generates structured rebuilds, drafts role-targeted cover letters, and runs interview preparation through a retrieval-grounded conversational assistant.

The Gemini integration is deliberately constrained — retrieval-augmented prompting keeps generated content anchored to the candidate's actual history rather than inventing credentials, which is the single most common failure mode in AI resume tooling.

**Impact:** turns a multi-tool, multi-hour application workflow into one session, shipping to **Web, Android, and Windows** from a single codebase.

`Flutter``Firebase``Riverpod``Gemini API``RAG`

<a href="https://github.com/ArsalanKaleem/Aestimo">   <img src="https://github-readme-stats.vercel.app/api/pin/?username=ArsalanKaleem&repo=Aestimo&theme=tokyonight&hide\_border=true&bg\_color=0D1117" alt="Aestimo" /> </a> ---

### ◆ F1 Vision — *Formula 1 telemetry, analyzed in real time.*

**A live motorsport analytics dashboard built on high-frequency telemetry streams.**

F1 Vision ingests live session data from the OpenF1 API alongside historical results from Jolpica, then renders driver comparisons, sector-level pace deltas, race analytics, and season-long statistics. The engineering challenge is throughput: rendering continuously updating telemetry without dropping frames, handled through selective Riverpod rebuilds and windowed data buffers.

An AI insight layer summarizes strategic patterns — stint degradation, undercut windows, pace convergence — in natural language on top of the raw numbers.

**Impact:** delivers live-session telemetry analysis normally locked behind proprietary broadcast tooling, as an open cross-platform dashboard.

`Flutter``Firebase``OpenF1 API``Jolpica API``Real-time Data`

<a href="https://github.com/ArsalanKaleem/F1-Vision">   <img src="https://github-readme-stats.vercel.app/api/pin/?username=ArsalanKaleem&repo=F1-Vision&theme=tokyonight&hide\_border=true&bg\_color=0D1117" alt="F1 Vision" /> </a> ---

### ◆ Documentium — *Documentation that keeps pace with the codebase.*

**An AI documentation generator that converts source repositories into structured, exportable technical documentation.**

Documentium walks a codebase, builds structural context, and dispatches analysis across parallel LLM calls to produce API references, module overviews, and project-level documentation. It is provider-agnostic by design — multiple LLM backends sit behind a single abstraction, so model choice becomes a configuration decision rather than a rewrite.

Built as a Flutter desktop and web application with Markdown export, keeping generated documentation in a format that lives in version control alongside the code it describes.

**Impact:** compresses the documentation pass on an unfamiliar codebase from days of manual writing to a single analysis run, with output committed as plain Markdown.

`Flutter``Dart``Firebase``Gemini API``Multi-Provider LLM``Parallel Agents`

<a href="https://github.com/ArsalanKaleem/Documentium">   <img src="https://github-readme-stats.vercel.app/api/pin/?username=ArsalanKaleem&repo=Documentium&theme=tokyonight&hide\_border=true&bg\_color=0D1117" alt="Documentium" /> </a> ---

### ◆ RHAI — *Applied AI workflow orchestration.*

**An AI automation layer that decomposes multi-step tasks into tool-invoking workflows with deterministic control flow.**

RHAI is built on the architecture pattern that separates reasoning from execution: an LLM plans and routes, while typed tools perform the actual work against real systems and return structured results. State is explicit and inspectable at each step, tool calls are validated before dispatch, and failures degrade into recoverable states rather than silent hallucination.

The design goal is practical automation — workflows that run reliably enough to be trusted with real inputs, rather than demos that work once. Retrieval grounding supplies domain context; the orchestration layer keeps the sequencing deterministic and auditable.

`Python``FastAPI``LLM Orchestration``Tool Calling``RAG``Agentic Workflows`

<a href="https://github.com/ArsalanKaleem/RHAI">   <img src="https://github-readme-stats.vercel.app/api/pin/?username=ArsalanKaleem&repo=RHAI&theme=tokyonight&hide\_border=true&bg\_color=0D1117" alt="RHAI" /> </a> ---

### ◆ CivicPing — *Closing the loop between citizens and local government.*`🚧 In Active Development`

**A civic technology platform for structured issue reporting, routing, and resolution tracking.**

Municipal complaints fail because there is no accountable channel and no visible state. CivicPing gives citizens a geotagged reporting flow, routes each report to the responsible department, and exposes status transitions publicly so resolution becomes verifiable rather than assumed.

The backend is a containerized FastAPI service handling routing logic, authentication, and department workflows, with Firebase supporting identity and real-time client sync. The Flutter client targets mobile and web so reporting works from wherever the problem is.

**Status:** active development — architecture and core reporting flow implemented, routing engine in progress.

`Flutter``Python``FastAPI``Docker``Firebase``REST APIs`

<a href="https://github.com/ArsalanKaleem/CivicPing">   <img src="https://github-readme-stats.vercel.app/api/pin/?username=ArsalanKaleem&repo=CivicPing&theme=tokyonight&hide\_border=true&bg\_color=0D1117" alt="CivicPing" /> </a> ---

## ▍Tech Stack

**Languages**

![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

**Frameworks & Application Architecture**

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)![Riverpod](https://img.shields.io/badge/Riverpod-4A90E2?style=for-the-badge&logo=flutter&logoColor=white)![GoRouter](https://img.shields.io/badge/GoRouter-0175C2?style=for-the-badge&logo=dart&logoColor=white)![Freezed](https://img.shields.io/badge/Freezed-13B9FD?style=for-the-badge&logo=dart&logoColor=white)![Dio](https://img.shields.io/badge/Dio-1F6FEB?style=for-the-badge&logo=dart&logoColor=white)![Hive](https://img.shields.io/badge/Hive-FFC107?style=for-the-badge&logo=databricks&logoColor=black)

**Backend & Data**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)![Cloud Firestore](https://img.shields.io/badge/Cloud_Firestore-F57C00?style=for-the-badge&logo=firebase&logoColor=white)![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)![REST APIs](https://img.shields.io/badge/REST_APIs-005571?style=for-the-badge&logo=fastapi&logoColor=white)![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)

**Artificial Intelligence**

![Gemini](https://img.shields.io/badge/Gemini_API-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)![RAG](https://img.shields.io/badge/RAG-00BFFF?style=for-the-badge&logo=databricks&logoColor=white)![AI Agents](https://img.shields.io/badge/AI_Agents-6E56CF?style=for-the-badge&logo=probot&logoColor=white)![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-1A7F64?style=for-the-badge&logo=openai&logoColor=white)

**GIS & Remote Sensing**

![Google Earth Engine](https://img.shields.io/badge/Google_Earth_Engine-4285F4?style=for-the-badge&logo=googleearth&logoColor=white)![QGIS](https://img.shields.io/badge/QGIS-589632?style=for-the-badge&logo=qgis&logoColor=white)![GeoPandas](https://img.shields.io/badge/GeoPandas-139C5A?style=for-the-badge&logo=pandas&logoColor=white)![Sentinel-2](https://img.shields.io/badge/Sentinel--2-0B3D91?style=for-the-badge&logo=esa&logoColor=white)![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

**Infrastructure & Tooling**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)![Android Studio](https://img.shields.io/badge/Android_Studio-3DDC84?style=for-the-badge&logo=androidstudio&logoColor=white)![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

---

## ▍GitHub Metrics

<p align="center">   <img height="165" src="https://github-readme-stats.vercel.app/api?username=ArsalanKaleem&show\_icons=true&theme=tokyonight&hide\_border=true&bg\_color=0D1117&include\_all\_commits=true&count\_private=true" alt="GitHub Stats" />   <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ArsalanKaleem&layout=compact&theme=tokyonight&hide\_border=true&bg\_color=0D1117&langs\_count=8" alt="Top Languages" /> </p> <p align="center">   <img src="https://streak-stats.demolab.com?user=ArsalanKaleem&theme=tokyonight&hide\_border=true&background=0D1117" alt="GitHub Streak" /> </p> <p align="center">   <img src="https://github-readme-activity-graph.vercel.app/graph?username=ArsalanKaleem&theme=tokyo-night&hide\_border=true&bg\_color=0D1117&area=true" alt="Activity Graph" width="100%" /> </p> <p align="center">   <img src="https://github-profile-trophy.vercel.app/?username=ArsalanKaleem&theme=tokyonight&no-frame=true&no-bg=true&column=7&margin-w=8" alt="Trophies" /> </p> ### Contribution Graph

<!--   SNAKE ANIMATION SETUP   1. Create .github/workflows/snake.yml in the ArsalanKaleem/ArsalanKaleem repo   2. Use Platane/snk@v3 with outputs:        dist/github-contribution-grid-snake.svg        dist/github-contribution-grid-snake-dark.svg?palette=github-dark   3. Push the result to an "output" branch on a daily cron schedule --> <p align="center">   <picture>     <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ArsalanKaleem/ArsalanKaleem/output/github-contribution-grid-snake-dark.svg" />     <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ArsalanKaleem/ArsalanKaleem/output/github-contribution-grid-snake.svg" />     <img alt="Contribution snake animation" src="https://raw.githubusercontent.com/ArsalanKaleem/ArsalanKaleem/output/github-contribution-grid-snake.svg" />   </picture> </p> ---

## ▍Open Source

Open source is where I do my most deliberate engineering — the code is read by strangers, so the architecture has to justify itself.

* **ForgeOS** is built to lower the entry barrier for first-time contributors: AI-guided issue matching, repository context, and a suggested approach before the first commit.
* I publish Flutter tooling and reusable architecture patterns from production work rather than tutorial code.
* Contributions welcome across all repositories — issues, discussions, and pull requests get reviewed.

<p align="center">   <img src="https://img.shields.io/badge/Open\_Source-Contributor-0D1117?style=for-the-badge&labelColor=161B22&color=00BFFF" alt="Open Source Contributor" />   <img src="https://img.shields.io/badge/PRs-Welcome-0D1117?style=for-the-badge&labelColor=161B22&color=00BFFF" alt="PRs Welcome" /> </p> ---

## ▍Research · Geospatial & Remote Sensing

Geospatial work is where software engineering meets measurable public impact.

**Sindh Water Access Index (SWAI)** applies remote sensing and spatial statistics to a development question with real policy weight: which settlements lack reliable access to drinking water, and by how much.

**Methodology**


| Stage              | Approach                                                                      |
| :----------------- | :---------------------------------------------------------------------------- |
| Acquisition        | Sentinel-2 collections via Google Earth Engine, cloud-masked and composited   |
| Preprocessing      | Raster normalization, reprojection, and clipping to administrative boundaries |
| Spatial modelling  | Distance-decay accessibility computation in GeoPandas across 5,159 villages   |
| Index construction | Multi-factor composite scoring, normalized and weighted in Pandas / NumPy     |
| Validation         | Cross-referenced against official government datasets                         |
| Output             | Publication-quality cartographic products in QGIS                             |

**Alignment:** UN Sustainable Development Goal 6 — Clean Water and Sanitation.

**Interests:** land-use classification, water resource monitoring, urban growth analysis, climate-resilience mapping.

---

## ▍Artificial Intelligence

I treat LLMs as a component in a system, not the system itself. Every AI feature I ship sits behind deterministic control flow, validated inputs, and grounded retrieval.

**Applied patterns**

* **Retrieval-Augmented Generation** — grounding model output in user and domain data to eliminate fabricated content (Aestimo, RHAI)
* **Multi-agent decomposition** — parallel specialized agents over sequential monolithic prompts (Documentium)
* **Tool-calling orchestration** — typed tool interfaces with validation before dispatch and structured results after (RHAI)
* **Provider abstraction** — model-agnostic interfaces so backend choice is configuration, not architecture
* **Context engineering** — structured prompting, token budgeting, and output schema enforcement

**Currently going deeper on:** multi-agent systems, LangGraph, Model Context Protocol (MCP), evaluation frameworks for non-deterministic outputs.

---

## ▍Writing

Long-form engineering notes on constraint solvers, Flutter architecture at scale, and geospatial pipelines.

<p align="center">   <img src="https://img.shields.io/badge/Blog-Coming\_Soon-0D1117?style=for-the-badge&labelColor=161B22&color=00BFFF" alt="Blog coming soon" /> </p> <!-- BLOG\_START — replace with blog-post-workflow GitHub Action output --> <!-- Planned:      • Modelling university timetabling as a CSP: constraints, propagation, and search      • Riverpod at scale: dependency graphs that survive a 50-screen application      • Building a village-level accessibility index with Earth Engine and GeoPandas      • RAG without hallucination: grounding strategies that actually hold --> <!-- BLOG\_END --> ---

## ▍Contact

Open to software engineering roles, research collaboration, and open source work in Flutter, applied AI, and geospatial systems.

<p align="center">   <a href="https://arsalankaleem.github.io/portfolio/"><img src="https://img.shields.io/badge/Portfolio-0D1117?style=for-the-badge&logo=firefoxbrowser&logoColor=00BFFF" alt="Portfolio" /></a>   <a href="https://linkedin.com/in/arsalankaleem"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>   <a href="mailto:arsalanabbasi.here@gmail.com"><img src="https://img.shields.io/badge/Email-0D1117?style=for-the-badge&logo=gmail&logoColor=EA4335" alt="Email" /></a>   <a href="https://github.com/ArsalanKaleem"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a> </p> <p align="center">   <sub><b>Flutter · Dart · Python · TypeScript · Artificial Intelligence · RAG · LLM Integration · AI Agents · Firebase · FastAPI · Docker · REST APIs · GIS · Remote Sensing · Google Earth Engine · QGIS · GeoPandas · Cross-Platform Development · System Design · Software Engineer</b></sub> </p> <p align="center">   <sub>Built to solve real problems, not to demo well.</sub> </p>
