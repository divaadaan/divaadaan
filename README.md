### Hi, I'm Dan 👋

I'm a software engineer focused on NLP and machine learning, and a hobbyist game developer. Lately I've been building with local LLMs and agent workflows, and leading the programming on a Unity/C# game project. I work iteratively, with AI agents as part of my development loop, and I like turning new research into working code. What I enjoy most is diving into an unfamiliar problem and getting straight to experiments.

---

#### Building

- **[grocery-optimizer](https://github.com/divaadaan/grocery-optimizer)**: *What can you cook from this week's grocery sales near you, within your dietary restrictions?* It ingests real flyer data for a postal code and filters it through a deterministic dietary gate built on curated product attributes, so no LLM or keyword match ever decides compliance. It then sorts deals into code-built trays with cross-store price comparison. A Chef agent plans dishes, and parallel SousChef agents write recipes in which every ingredient cites a real deal. Output is validated, repaired in code where that's safe, and costed from those citations. Quality is measured with a record-and-replay eval harness over frozen data snapshots (the compliance gate passed 14/14 on the latest live runs) and 1,584 deterministic tests. Built with FastAPI + PostgreSQL, React/TypeScript, local Ollama and the Hugging Face router. **[Screenshot walkthrough →](https://github.com/divaadaan/grocery-optimizer/blob/main/docs/walkthrough/README.md)**, no install needed. Flyer ingestion builds on [FriendlyUser/flipp_flyer_parser](https://github.com/FriendlyUser/flipp_flyer_parser).
- **[ollama-api](https://github.com/divaadaan/ollama-api)** — FastAPI service for local LLM development, used to test a `smolagents` agent against a self-hosted model.

#### Client & commercial work

Some of my work is under private repos rather than missing entirely — client engagements and product work I keep private per the service agreement, not because there's nothing to show. Happy to walk through the details or share a demo on request.

- Built a hybrid ML/LLM automated essay scoring pipeline for an edutech client — private under our agreement, but I can talk through the architecture and tradeoffs in an interview.

#### Learning in public

I use forks to work through courses, textbooks, and other people's codebases hands-on rather than just reading — these are exercises and adaptations, not original projects, but they're where a lot of the actual skill-building happens:

- **[llm-from-scratch](https://github.com/divaadaan/llm-from-scratch)** — working through building an LLM from first principles
- **[DLTF](https://github.com/divaadaan/DLTF)** — *Deep Learning with TensorFlow and Keras* (Packt), worked exercises
- **[dj4e](https://github.com/divaadaan/dj4e)** — *Django for Everybody* coursework
- **[Full-Stack-Development-with-Spring-Boot-3-and-React](https://github.com/divaadaan/Full-Stack-Development-with-Spring-Boot-3-and-React-Fourth-Edition)** — Spring Boot 3 + React, worked exercises

#### Stack

Python · FastAPI · PostgreSQL · TypeScript/React · Java · C#/Unity · TensorFlow/Keras · local LLM tooling (Ollama, agents)

---
