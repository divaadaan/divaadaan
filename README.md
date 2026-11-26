### Hi, I'm Dan 👋

I'm a software engineer focused on NLP and machine learning, and a hobbyist game developer. Lately I've been building with local LLMs and agent workflows, measuring how closely LLM graders agree with human ones, and leading the programming on a Unity/C# game project. I work iteratively, with AI agents as part of my development loop, and I like turning new research into working code. What I enjoy most is diving into an unfamiliar problem and getting straight to experiments.

---

#### Building

- **[grocery-optimizer](https://github.com/divaadaan/grocery-optimizer)**: *What can you cook from this week's grocery sales near you, within your dietary restrictions?* **[Screenshot walkthrough →](https://github.com/divaadaan/grocery-optimizer/blob/main/docs/walkthrough/README.md)**. This project ingests real flyer data for a postal code and filters it through a deterministic dietary gate built on curated product attributes. It then sorts deals into code-built trays with cross-store price comparison. A Chef agent plans dishes, and parallel SousChef agents write recipes in which every ingredient cites a real deal. Output is validated, repaired in code where that's safe, and costed from those citations. Quality is measured with a record-and-replay eval harness over frozen data snapshots. Built with FastAPI + PostgreSQL, React/TypeScript, local Ollama and the Hugging Face router. Flyer ingestion builds on [FriendlyUser/flipp_flyer_parser](https://github.com/FriendlyUser/flipp_flyer_parser).
- **[guide-exemplars](https://github.com/divaadaan/guide-exemplars)**: *LLMs don't grade essays the way people do. How close can you get?* **[Screenshot walkthrough →](https://github.com/divaadaan/guide-exemplars/blob/main/docs/walkthrough/README.md)**. Out of the box, LLM graders score short essays too high, mark long ones down for minor slips, and bunch their scores in the middle of the scale. This repo narrows that gap two ways. A Bayesian-optimization search, adapted from the GUIDE paper, picks the few-shot examples that sit on the boundaries between score levels, and rewrites each rationale to say why the example earns its score and not the neighbouring one. A feature grader has the LLM count rubric evidence, turns the counts into per-word rates, and fits a small ordinal model to human scores. The hybrid combines the two. On ASAP essays the hybrid matches the human raters' agreement with each other (QWK 0.597 vs 0.599), where the exemplar search alone reaches 0.380. Every LLM call goes through a response cache and a hard spend cap, so the benchmark replays byte for byte, and 228 offline tests run with no network. Ships as a library, CLI and FastAPI service with a live dashboard. Built with Python, numpy/scikit-learn, FastAPI + SQLite, vanilla JS + Plotly, and OpenAI or any OpenAI-compatible server.
- **[ollama-code-agent](https://github.com/divaadaan/ollama-api)**: my project for the Hugging Face Agents Course (certified, 2025). A `smolagents` code agent on a local Ollama model, served by FastAPI, with web, file, OCR and speech tools, a second LLM pass that reviews each answer and retries on a fail, and optional OpenTelemetry + Prometheus monitoring. A per-tool benchmark endpoint and 38 offline tests check it.

#### Learning repos

These are forks of courses, textbooks, and other people's codebases — these are exercises and adaptations, not original projects:

- **[DLTF](https://github.com/divaadaan/DLTF)** — *Deep Learning with TensorFlow and Keras* (Packt), worked exercises
- **[dj4e](https://github.com/divaadaan/dj4e)** — *Django for Everybody* coursework
- **[Full-Stack-Development-with-Spring-Boot-3-and-React](https://github.com/divaadaan/Full-Stack-Development-with-Spring-Boot-3-and-React-Fourth-Edition)** — Spring Boot 3 + React, worked exercises

#### Stack

Python · FastAPI · PostgreSQL · TypeScript/React · Java · C#/Unity · TensorFlow/Keras · scikit-learn · local LLM tooling (Ollama, agents)

---
