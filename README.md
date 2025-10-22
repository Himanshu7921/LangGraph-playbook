# LangGraph Playbook

> “A practical LangGraph playbook to plan, build, and learn - documented like an engineer.”

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.9%2B-blue.svg)](https://www.python.org/)
[![LangGraph](https://img.shields.io/badge/LangGraph-playbook-000000.svg)](https://langchain-ai.github.io/langgraph/)
[![AI Agents](https://img.shields.io/badge/agents-multi--agent--system-orange.svg)]()
[![RAG](https://img.shields.io/badge/RAG-RetrievalMind-success.svg)](https://github.com/Himanshu7921/RetrievalMind)
[![Status](https://img.shields.io/badge/status-learning--in--public-brightgreen.svg)]()
[![Docs](https://img.shields.io/badge/docs-cheatsheets%20%26%20journal-informational.svg)](#documentation)

This repository is my structured, professional playbook for learning and applying **LangGraph**, building on prior **LangChain** experience. It’s optimized for small, focused experiments; clear documentation; and repeatable patterns that scale into mini-projects.

---

## Table of contents

- Overview and goals
- Repository structure
- Documentation
- Experiments and how to run
- Mini-projects and comparisons
- Daily workflow (for fast iteration)
- Roadmap & progress tracker
- How to use this as a template
- License and contact

---

## Repository structure

```
docs/
   features.md              # Feature tracker table (single source of truth)
   cheatsheets/
      nodes_and_edges.md
      agent_execution.md
      graph_patterns.md
   notes/
      concepts.md            # High-level notes and concepts
   journal/
      2025-10.md             # Monthly journal (daily entries)

experiments/
   README.md                # How to run and add new experiments
   node_chaining/
      README.md
      node_chaining.py
   planner_agent/
      README.md
      planner_agent.py

mini_projects/
   README.md
   qna_bot/
      README.md
   workflow_automation/
      README.md

comparisons/
   langgraph_vs_langchain.md

archive/                   # Snapshots of older experiments
   README.md

templates/
   experiment_template.md
   project_template.md
   journal_template.md

.gitignore                 # Python/VSCodium/Notebook friendly ignores
```

---
## Documentation

This repo is designed to be your “second brain” for LangGraph.

- Cheatsheets: `docs/cheatsheets/` — terse, visual, copy-ready snippets.
- Notes: `docs/notes/concepts.md` — high-level ideas, definitions, mental models.
- Journal: `docs/journal/2025-10.md` — one small entry per day; template included.
- Feature tracker: `docs/features.md` — single source of truth for progress.

Guidelines
- Keep entries short. Link to experiments for detail.
- Prefer code snippets and ASCII sketches over prose when possible.
- Move stale versions into `archive/` with a date prefix.

---

## Experiments and how to run

Each experiment is small and runnable. Start with:

- `experiments/node_chaining/node_chaining.py`
- `experiments/planner_agent/planner_agent.py`

Run (Windows PowerShell):

```powershell
python .\experiments\node_chaining\node_chaining.py
python .\experiments\planner_agent\planner_agent.py
```

Add a new experiment
1) Create `experiments/<topic>/`
2) Copy `templates/experiment_template.md` to `<topic>/README.md`
3) Add `<topic>.py` or a notebook
4) Log results in the README and update `docs/features.md`

---

## Mini-projects and comparisons

- Mini-projects: sketch slightly larger ideas and wire multiple nodes together.
- Comparisons: `comparisons/langgraph_vs_langchain.md` for side-by-side takeaways.

Suggested mini-project ideas
- Q&A bot with retrieval + reasoning
- Workflow automation (fetch → process → summarize)
- Multi-agent planner simulation

---

## Daily workflow (fast iteration)

1) Journal: open `docs/journal/2025-10.md`, copy the template for today, and write 3–6 bullets.
2) Tracker: update `docs/features.md` (status, one-line note, date).
3) Experiment: add or iterate a tiny script in `experiments/` and link back in the journal.
4) Snapshot: archive older versions you want to keep in `archive/`.
5) Overview: update `structure.txt` via `generate_file_structure.py` for a current tree.

Tips
- Keep scope minimal; finish something daily.
- Log inputs/outputs to make debugging transitions trivial.
- Prefer repeatable, composable patterns (routers, fan-in/out, retries).

---

## Roadmap & progress tracker

Current focus
- [x] Basics of LangGraph
- [ ] Graph Nodes & Connections
- [ ] Agent Planning & Execution
- [ ] Integrating External APIs
- [ ] Advanced Pipelines

Track granular progress in `docs/features.md` (✅ Done | 🔄 WIP | 🧪 Testing | ⏳ Planned | ❌ Blocked).

---

## How to use this as a template

This repository includes a reusable generator prompt at the root:
- `folder_generation_prompt.txt` — feed this to any AI agent to recreate the structure and files with exact contents. It also defines the expected `structure.txt` tree.

---

## License

This project is licensed under the MIT License. See `LICENSE` for details.

---

## Contact

- Email: himanshusr451tehs@gmail.com
- LinkedIn: https://www.linkedin.com/in/himanshu-singh-552411251/