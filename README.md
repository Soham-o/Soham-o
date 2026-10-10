<div align="center">

<img src="header.svg" alt="Soham Panda: computer science student working on AI systems and developer tooling" width="100%"/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Soham_Panda-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/soham-panda-a90720336/)
[![Email](https://img.shields.io/badge/Email-sohampanda95599%40gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:sohampanda95599@gmail.com)

</div>

## About me

I'm a computer science student at **SGT University** in India. I build tools in
**Python** that put AI to practical use: desktop assistants, decision-support
dashboards and small automations. Lately I've also been making focused fixes in
other people's open-source projects.

What I care about in my own projects: running locally when possible, degrading
gracefully when a dependency is missing, and having tests that pin down the
behaviour I claim.

## Featured projects

### [Cursor Bite](https://github.com/Soham-o/cursor_bite) · working (Windows)

A local-first Windows assistant that opens a radial menu at your mouse cursor
when you press a hotkey, so you can translate, explain, summarize, rewrite, OCR
or search the text you've selected without switching apps.

- **Built:** native `RegisterHotKey` listener, a PyQt6 radial menu and result
  panel, clipboard-safe selection capture, and a privacy gateway that blocks or
  asks consent before sensitive text leaves the machine (web search only).
  Every optional engine loads lazily and fails safe.
- **Tech:** Python, PyQt6, pywin32, Ollama, Argos Translate, Tesseract.
- **Evidence:** about 300 pytest tests (unit, integration and security) and
  GitHub Actions CI on Windows.
- **Limits:** Windows only. Read Aloud is planned, not built.

### [AirTwin X](https://github.com/Soham-o/AirTwin-X) · prototype

A Streamlit dashboard that breaks a city's AQI down by likely source, ranks
eight municipal interventions with a weighted multi-criteria score, simulates
combined interventions with overlap-compounding instead of naive addition, and
estimates health and economic effects.

- **Tech:** Python, Streamlit, Folium, Plotly, OSMnx/NetworkX, XGBoost,
  Stable-Baselines3; WAQI, Open-Meteo and OpenStreetMap data.
- **Evidence:** 27 pytest tests for determinism, ranking and simulation bounds.
- **Limits:** model weights are fixed assumptions, the forecast model is
  trained on synthetic data, and live sensor data needs a WAQI token
  (otherwise it uses simulated data).

### [EarthShare](https://github.com/Soham-o/EarthShare) · prototype

A carbon-footprint tracker with a deterministic emissions engine, a FastAPI
backend and a Next.js frontend.

- **Tech:** Python, FastAPI, pytest; TypeScript, Next.js/React, Vitest.
- **Evidence:** backend and frontend test suites, including security and
  accessibility tests.

## Open-source contributions

Merged pull requests to projects maintained by other people:

| Project | Pull request | What it changed |
|---|---|---|
| [hermes-labs-ai/lintlang](https://github.com/hermes-labs-ai/lintlang) | [#88](https://github.com/hermes-labs-ai/lintlang/pull/88) · merged | The YAML config parser now rejects non-string tool names with a clear `tools[i].name must be a string` error instead of failing with an internal `AttributeError`, with a regression test (fixes #87). |
| [1jehuang/jcode](https://github.com/1jehuang/jcode) | [#1645](https://github.com/1jehuang/jcode/pull/1645) · merged | The Anthropic provider (Rust) now drops orphaned native web-search blocks left by interrupted turns before replaying history, which otherwise caused the API to reject the whole request; includes tests. |

All of my public pull requests:
[github.com/pulls?q=author:Soham-o](https://github.com/pulls?q=is%3Apr+author%3ASoham-o+is%3Apublic)

## Other work

- **[PersonaLearn](https://github.com/Soham-o/PersonaLearn)**: team project
  (Team Innovsphere, 5 members) built in a 3-hour sprint. A Streamlit app that
  uses Gemini to explain study topics through analogies from a learner's
  interests and quizzes them on the result.
- **Machine-learning notebooks**:
  [movie recommender](https://github.com/Soham-o/Movie_Recommender_System),
  [Spotify genre clustering](https://github.com/Soham-o/Spotify_Songs_Genre_Segmentation),
  [fake-news detection](https://github.com/Soham-o/Fake-News-Detection-),
  using scikit-learn (cosine similarity, k-means, logistic regression) and pandas.

## Tools I've used in public projects

**Languages:** Python (most of my work), TypeScript/JavaScript; one merged fix in Rust<br/>
**Apps & UI:** PyQt6, Streamlit, Next.js/React<br/>
**Backend & data:** FastAPI, pandas, NumPy, scikit-learn<br/>
**AI & ML:** Ollama (local LLMs), Google Gemini API, PyTorch / Stable-Baselines3, XGBoost<br/>
**Engineering:** pytest, GitHub Actions, Git, Linux

## Currently exploring

Multi-agent frameworks such as CrewAI, voice agents, and deploying Python
services to Google Cloud. These aren't in my public repositories yet.

## Get in touch

I'm open to open-source and research collaboration, freelance AI or
automation projects, and full-time roles. The best way to reach me is
[email](mailto:sohampanda95599@gmail.com) or
[LinkedIn](https://www.linkedin.com/in/soham-panda-a90720336/).

<div align="center">

<img src="footer.svg" alt="Footer: automate everything, build once, let it run forever. sohampanda95599@gmail.com, github.com/Soham-o" width="100%"/>

</div>
