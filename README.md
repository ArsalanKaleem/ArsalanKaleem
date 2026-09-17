> **I build systems where correctness matters more than novelty.**
>
> My work sits at the intersection of software engineering, applied artificial intelligence,
> geospatial computation, and empirical research — with a recurring question:
>
> **Can we turn an ambiguous real-world problem into a system whose assumptions, data,
> failure modes, and conclusions can all be inspected?**

---

# `01` · RESEARCH / ENGINEERING THESIS

I am interested in the space between **research that never becomes software** and **software that never questions its assumptions**.

My projects generally follow the same pipeline:

```text
REAL-WORLD PROBLEM
       │
       ▼
┌─────────────────────┐
│ Formalize            │
│ assumptions          │
│ constraints          │
│ measurable outcomes  │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Build the pipeline   │
│ data → computation   │
│ state → interface    │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Validate             │
│ controls             │
│ sensitivity          │
│ failure modes        │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Ship                 │
│ reproducible system  │
│ documentation        │
│ evidence             │
└─────────────────────┘
```

The result is not simply an application, model, or analysis.

It is a **reproducible system with an explicit epistemic boundary**.

---

# `02` · WHAT I BUILD

### `SYSTEMS`

Production-oriented cross-platform applications designed around explicit boundaries, deterministic state transitions, offline resilience, and maintainable architecture.

**Flutter · Dart · Riverpod · Freezed · GoRouter · Clean Architecture · Firebase · REST · GraphQL**

### `AI`

AI systems where language models are treated as probabilistic components rather than sources of truth.

**RAG · Agentic Workflows · Structured Tool Calling · Multi-Provider LLMs · Gemini · Evaluation · AI Safety**

### `GEOSPATIAL`

Spatial pipelines for questions that disappear when data is aggregated too aggressively.

**Google Earth Engine · Sentinel-2 · GeoPandas · QGIS · OSMnx · NetworkX · Remote Sensing**

### `RESEARCH`

Empirical work focused on measurement validity, controls, reproducibility, and identifying where apparently reasonable methodologies produce misleading conclusions.

**Statistics · Experimental Design · Spatial Analysis · Constraint Solving · Reproducible Pipelines**

---

# `03` · SELECTED WORK

## 💧 SWAI

### Sindh Water Access Index

A village-level drinking-water accessibility pipeline covering **5,159 settlements in Sindh** using open satellite and geospatial data.

The interesting part is not the index itself.

It is the methodological failure discovered during construction:

> A conventional formulation could make one of Pakistan's driest districts appear to have the strongest access.

The project documents the mathematical reason, the correction, and the complete geospatial pipeline rather than hiding the uncomfortable result.

**Stack**

`Python``Google Earth Engine``GeoPandas`
`Sentinel-2``QGIS``Spatial Statistics`

[View repository](https://github.com/ArsalanKaleem/Sindh-Water-Access-index-SWAI-)

## 🏥 RHAI

### Rural Healthcare Accessibility Index

A spatial accessibility model for rural healthcare across Sindh.

Instead of drawing circles around facilities, the analysis considers **actual road-network travel** and investigates how incomplete open geospatial data can distort apparent accessibility.

The project treats missing facilities and incomplete road data as measurement problems — not footnotes.

**Stack**

`Python``OSMnx``NetworkX`
`GeoPandas``QGIS``Spatial Analysis`

[View repository](https://github.com/ArsalanKaleem/Rural-Healthcare-Accessibility-Index--RHAI-)

## 🧠 UNLEARNING AUDIT

### Never-Taught Controls in LLM Unlearning

An empirical audit of whether apparent LLM unlearning represents actual knowledge removal or merely behavioral suppression.

The central experimental idea is deliberately simple:

**What happens when the same diagnostic is applied to information the model was never taught?**

The work uses preregistered thresholds, control conditions, and CPU-only reproducibility to test whether commonly used diagnostics actually measure what they claim to measure.

**Stack**

`Python``PyTorch``Statistics`
`Experimental Design``AI Safety`

[View repository](https://github.com/ArsalanKaleem/unlearning-audit)

## 🏎️ F1-VISION

### Real-Time Motorsport Analytics

A research-grade Flutter telemetry environment that reconstructs races lap-by-lap rather than reducing them to a leaderboard.

Live telemetry, race control, tyre evolution, strategy analysis, driver comparison, derived overtakes, race replay, and season-wide analytics are brought into one interface.

Built entirely around free public data sources.

**Stack**

`Flutter``Riverpod``Isar`
`OpenF1``Jolpica``Telemetry`

[View repository](https://github.com/ArsalanKaleem/F1-Vision)

## 🎬 SIMUL

### Synchronized Watch-Party Infrastructure

A six-platform real-time application for synchronized YouTube watching with voice chat, screen sharing, audio, reactions, and multiplayer interaction.

The engineering challenge is synchronization under imperfect networks — not merely putting a video player beside a chat window.

Includes documented Firestore security rules and explicit trust-boundary analysis.

**Stack**

`Flutter``Firebase``LiveKit`
`WebRTC``Real-Time Sync`

[View repository](https://github.com/ArsalanKaleem/simul-watch-together-app)

## 📄 DOCUMENTUM

### Multi-Agent Documentation Infrastructure

A provider-agnostic documentation system that coordinates AI agents over a codebase to generate:

* architecture documentation
* API references
* README material
* changelogs
* project knowledge

A persistent semantic **Project Brain** allows generated documentation to evolve with the underlying codebase.

**Stack**

`Flutter``Multi-Agent AI`
`RAG``LLM Orchestration``REST`

[View repository](https://github.com/ArsalanKaleem/Documentum)

## 🔭 FORGEOS

### AI-Assisted Open Source Onboarding

A tool designed around the first-contribution problem:

**finding an issue is easy; understanding whether you can actually solve it is not.**

ForgeOS filters GitHub issues and uses AI to explain the problem, expected skills, difficulty, and possible direction without simply giving away the implementation.

No account. No proprietary backend. Free public APIs.

**Stack**

`Flutter``Riverpod``Gemini`
`GitHub APIs``Offline-first`

[View repository](https://github.com/ArsalanKaleem/forge-os)

## 💼 AESTIMO

### AI Career & Resume Intelligence

A grounded career assistant where downstream features are constrained by the user's actual resume rather than generic career advice.

Includes:

`ATS analysis` · `resume intelligence` · `grounded chat` · `job matching` · `cover letters` · `interview preparation` · `live mock interviews`

One codebase targeting Android, Web, and Windows.

**Stack**

`Flutter``Gemini``Firebase`
`RAG``Riverpod`

[View repository](https://github.com/ArsalanKaleem/Aestimo)

## 🔐 WEBSITE SECURITY ASSESSMENT

### Non-Destructive Security Analysis

A modular FastAPI security assessment pipeline covering TLS configuration, HTTP security headers, DNS/email posture, application configuration, and vulnerability correlation.

The design principle is explicit:

> **Assess. Explain. Remediate. Never exploit.**

SSRF and DNS-rebinding protection form a centralized security boundary around outbound assessment operations.

**Stack**

`Python``FastAPI``Docker`
`OSV``NVD``CISA KEV`

## 💬 NUNTIUS

### Privacy-First WhatsApp Analytics

A completely on-device analytics system for exported WhatsApp conversations.

No account.
No server.
No analytics SDK.

Designed for real-world exports, including large conversations, iOS/Android format differences, code-switched Roman Urdu/Hindi, search, dashboards, Wrapped-style storytelling, and PDF reports.

**Stack**

`Flutter``On-Device Processing`
`NLP``Data Visualization`

[View repository](https://github.com/ArsalanKaleem/Nuntius)

---

# `04` · ENGINEERING PRINCIPLES

### 01 — Determinism before intelligence

If a rule can be encoded deterministically, it should not be delegated to a language model.

```text
deterministic computation
        +
validated data
        +
structured tools
        +
bounded model reasoning
        =
more trustworthy AI systems
```

### 02 — Architecture is a constraint, not decoration

I prefer systems where dependencies point inward and boundaries are visible.

```text
Presentation
     ↓
Application
     ↓
Domain
     ↓
Infrastructure
```

State should be observable.

Side effects should be isolated.

Business rules should be testable without rendering a screen.

### 03 — Offline is a design decision

Network failure is not an exceptional event.

Applications should know what they can do without connectivity, preserve local state, and synchronize deliberately rather than assuming the network is always available.

### 04 — Data provenance matters

A polished visualization does not make weak data strong.

For analytical systems I care about:

* source provenance
* spatial resolution
* temporal coverage
* missingness
* measurement error
* assumptions
* sensitivity
* validation
* reproducibility

### 05 — Negative results are results

If a methodology produces a surprising conclusion, the first response should be:

**audit the pipeline.**

Not:

**hide the result.**

---

# `05` · TECHNOLOGY

### Languages

`Dart` · `Python` · `TypeScript`

### Application Engineering

`Flutter` · `Riverpod` · `Freezed` · `GoRouter`
`Clean Architecture` · `Offline-first Systems`

### Artificial Intelligence

`RAG` · `Agentic Workflows` · `Structured Tool Calling`
`Gemini API` · `Multi-provider LLM Orchestration`
`AI Evaluation` · `AI Safety`

### Data / Scientific Computing

`Pandas` · `NumPy` · `scikit-learn`
`PyTorch` · `Statistics` · `Experimental Design`

### GIS / Earth Observation

`Google Earth Engine` · `GeoPandas` · `QGIS`
`OSMnx` · `NetworkX` · `Sentinel-2`
`Remote Sensing` · `Spatial Analysis`

### Infrastructure

`Firebase` · `FastAPI` · `Docker`
`REST` · `GraphQL` · `LiveKit` · `WebRTC`
`GitHub Actions` · `CI/CD`

---

# `06` · RESEARCH DIRECTIONS

I am particularly interested in problems where **software engineering becomes a method of inquiry**.

### 🌍 Geospatial Inequality

How much can open satellite, population, road-network, and administrative data tell us about access to essential services — and where does that measurement break?

### 🧠 AI Reliability

How do we distinguish actual model capabilities from artifacts of prompting, evaluation design, data leakage, benchmark construction, or behavioral suppression?

### 🧩 Constraint Systems

How can messy institutional rules be translated into explicit mathematical constraints and solved deterministically?

### 🤖 Agentic Software

What happens when language models stop being chat interfaces and become bounded components inside larger software systems?

### 🔬 Reproducible Engineering

How do we build research software that someone else can actually run, inspect, challenge, and reproduce?

---

# `07` · THE COMMON THREAD

Different projects.

Same philosophy.

```text
                  ┌────────────────────┐
                  │  REAL WORLD        │
                  │  PROBLEM           │
                  └─────────┬──────────┘
                            │
              ┌─────────────▼─────────────┐
              │       FORMALIZATION       │
              │ constraints · assumptions │
              └─────────────┬─────────────┘
                            │
           ┌────────────────▼────────────────┐
           │             SYSTEM              │
           │ software · data · models · GIS  │
           └────────────────┬────────────────┘
                            │
              ┌─────────────▼─────────────┐
              │        VALIDATION         │
              │ controls · tests · audits │
              └─────────────┬─────────────┘
                            │
                 ┌──────────▼──────────┐
                 │     REPRODUCIBLE    │
                 │      RESULT         │
                 └─────────────────────┘
```

I am less interested in building another demonstration of what technology *can* do.

I am more interested in determining:

**what it actually does, under which assumptions, and whether the result survives inspection.**

---

# `08` · CURRENTLY

```text
┌──────────────────────────────────────────────────────────────┐
│                                                              │
│  BUILDING                                                    │
│  ├── production Flutter systems                              │
│  ├── AI-assisted developer infrastructure                    │
│  ├── geospatial research pipelines                           │
│  └── reproducible analytical tooling                         │
│                                                              │
│  STUDYING                                                    │
│  ├── AI evaluation & reliability                             │
│  ├── spatial accessibility                                   │
│  ├── remote sensing                                          │
│  ├── constraint optimization                                 │
│  └── empirical research methodology                           │
│                                                              │
│  PRINCIPLE                                                   │
│  └── make the assumptions inspectable                         │
│                                                              │
└──────────────────────────────────────────────────────────────┘
```

---

# `09` · OPEN SOURCE

Most of the interesting engineering problems become more interesting when somebody else can inspect the solution.

I publish systems, experiments, datasets, methodologies, and tooling with an emphasis on:

* reproducibility
* architectural clarity
* explicit limitations
* documented assumptions
* useful failure modes
* practical deployment

If a project can teach another engineer something, I want the repository to contain enough context for them to understand **why** it was built — not only **how**.

---

# `10` · ELSEWHERE

---

### `BUILD · MEASURE · QUESTION · REPRODUCE`
