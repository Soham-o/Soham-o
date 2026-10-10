<div align="center">

<img src="header.svg" alt="Soham Panda: computer science student working on AI systems and developer tooling" width="100%"/>

### I build practical AI software: tools that run on your own machine, show their reasoning, and keep working when a piece is missing.

[Projects](#featured-projects) · [Open source](#open-source-contributions) · [Toolbox](#toolbox) · [Contact](#lets-build-something)

</div>

<br/>

Hi, I'm **Soham**, a computer science student at **SGT University** in India.
Most of my projects start with a small, specific frustration. One is switching
tabs just to translate a sentence. Another is a city air-quality dashboard that
shows a number but not what to do about it. I like turning those into working
software, then writing the tests that prove it does what the README says.

Lately I've also been reading other people's codebases closely enough to fix
real bugs in them. Two of those fixes have been merged.

<br/>

## Featured projects

### ⌨️ [Cursor Bite](https://github.com/Soham-o/cursor_bite)
**A radial AI menu that opens at your mouse cursor, anywhere in Windows.**

<a href="https://github.com/Soham-o/cursor_bite"><img src="assets/cursor-bite.png" alt="Cursor Bite's radial menu with Translate highlighted, next to its keyboard shortcuts: Ctrl+Alt+B to open, then keys 1 to 8 for Translate, Summarize, Explain, Search Web, Settings, Capture OCR, Rewrite and Ask AI" width="100%"/></a>

Select text in any app, press `Ctrl+Alt+B`, and translate, explain, summarize,
rewrite or OCR it without leaving the window. Everything except web search
runs locally. A privacy gateway checks for secrets and personal data, and asks
before anything sensitive leaves the machine.

**Interesting bits:** a native Windows hotkey with no keyboard hooks · a menu
that never waits on clipboard capture · every engine is optional and loads
lazily, so a bare install still starts · about 300 pytest tests and Windows CI

`Python` `PyQt6` `pywin32` `Ollama` `Argos Translate` `Tesseract` · **Status:** working on Windows

<br/>

### 🌫️ [AirTwin X](https://github.com/Soham-o/AirTwin-X)
**Air-quality decision support that asks "what should the city do?", not just "how bad is it?".**

<a href="https://github.com/Soham-o/AirTwin-X"><img src="assets/airtwin-x.png" alt="AirTwin X pipeline: live data from WAQI, Open-Meteo, NASA FIRMS and OpenStreetMap feeds source attribution, then intervention ranking, scenario simulation, health and economic impact, and a rule-based Mayor Copilot" width="100%"/></a>

A Streamlit prototype that estimates which sources are driving a city's AQI,
ranks eight interventions, and simulates combining them. Overlapping policies
**compound instead of adding up**, and the combined drop is capped at 85%. The
"Mayor Copilot" answers questions only from those computed results, with no
LLM, so every number can be traced.

`Python` `Streamlit` `OSMnx` `XGBoost` `Folium` `Plotly` · **Status:** prototype; 29 tests run in GitHub Actions; model weights are stated assumptions

<br/>

### 🌍 [EarthShare](https://github.com/Soham-o/EarthShare)
**A carbon tracker built around owning your footprint, not just watching it.**

<a href="https://github.com/Soham-o/EarthShare"><img src="assets/earthshare.png" alt="EarthShare dashboard showing a daily check-in, a carbon score ring at 565, 520 kg of CO2 this month, reduction potential and yearly projections" width="100%"/></a>

Log daily activities, get deterministic emission estimates, and pick climate
actions that show up in your projections. A full-stack app with JWT auth, rate
limiting and security headers. GitHub Actions runs the backend tests (85 passed,
1 skipped), the frontend tests (21 passed, including accessibility checks) and a
production build.

`FastAPI` `Next.js` `TypeScript` `pytest` `Vitest` · **Status:** prototype, built for a hackathon

<br/>

<details>
<summary><b>More projects</b></summary>
<br/>

- **[PersonaLearn](https://github.com/Soham-o/PersonaLearn)**: a team project (Team Innovsphere, 5 people, built in 3 hours). It uses Gemini to explain study topics through analogies from a learner's interests, then quizzes them.
- **ML notebooks**: [movie recommender](https://github.com/Soham-o/Movie_Recommender_System) (cosine similarity), [Spotify genre clustering](https://github.com/Soham-o/Spotify_Songs_Genre_Segmentation) (k-means) and [fake-news detection](https://github.com/Soham-o/Fake-News-Detection-) (TF-IDF and logistic regression).

</details>

## Open-source contributions

Merged pull requests to projects maintained by other people:

| Project | What I fixed |
|---|---|
| **[lintlang](https://github.com/hermes-labs-ai/lintlang)** · [#88](https://github.com/hermes-labs-ai/lintlang/pull/88) ✅ merged | Non-string tool names in YAML configs crashed the parser with an internal `AttributeError`. Now they get a clear `tools[i].name must be a string` error and a regression test (fixes #87). |
| **[jcode](https://github.com/1jehuang/jcode)** · [#1645](https://github.com/1jehuang/jcode/pull/1645) ✅ merged | An interrupted turn could leave an orphaned web-search block in the saved history, and replaying it made the Anthropic API reject the whole request. The Rust provider now drops those blocks before replay, with tests. |

[See all my public pull requests →](https://github.com/pulls?q=is%3Apr+author%3ASoham-o+is%3Apublic)

## Toolbox

What I've actually used in the projects above:

| | |
|---|---|
| **Languages** | Python · TypeScript · JavaScript · Rust (one merged fix) |
| **Apps & UI** | PyQt6 · Streamlit · Next.js / React |
| **Backend & data** | FastAPI · pandas · NumPy · scikit-learn · OSMnx |
| **AI & ML** | Ollama · Gemini API · XGBoost · Stable-Baselines3 / PyTorch |
| **Engineering** | pytest · Vitest · GitHub Actions · Git · Linux |

**Exploring next:** multi-agent frameworks such as CrewAI, voice agents, and deploying Python services to Google Cloud.

## Let's build something

I'm open to open-source and research collaboration, freelance AI or automation
projects, and full-time roles. If one of these projects overlaps with something
you're working on, I'd like to hear about it.

<div align="center">

[![Email](https://img.shields.io/badge/Email-sohampanda95599%40gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:sohampanda95599@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Soham_Panda-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/soham-panda-a90720336/)

<img src="footer.svg" alt="Footer: automate everything, build once, let it run forever. sohampanda95599@gmail.com, github.com/Soham-o" width="100%"/>

</div>
