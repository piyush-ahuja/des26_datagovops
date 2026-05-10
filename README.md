# DataGovOps

**Governing GenAI: DataGovOps When AI Is Your Biggest Data Consumer**

Presented at [Data Engineering Summit 2026](https://des.analyticsindiamag.com/agenda/) · Bangalore

---

## The thesis

> Your biggest data consumer is no longer human. Your governance was built for humans. That gap is your next incident.

For twenty years, enterprise governance assumed the primary data consumer was human — an analyst writing SQL, a user opening a dashboard, an engineer building a pipeline. GenAI changes that assumption. AI agents consume data through prompts, embeddings, vector stores, tools, memory, and downstream outputs — continuously, at machine speed, and without the deterministic behavior traditional controls were designed around.

**DataGovOps** is governance engineered into the AI data path.

---

## The framework

Four engineering moves. Four verbs.

| | Enforce | Decide | Trace | Verify |
|---|---|---|---|---|
| **Move** | Policy as code | Intent + consent | Source-to-output lineage | Govern the governor |
| **Shift** | Governance rules in Git, reviewed in PRs, enforced in CI/CD | Access scoped by what the agent is trying to do, consent as a query-time filter | Classification tags propagate from source through embeddings to agent output | AI-assisted classification with human gates, eval sets, and deterministic fallbacks |
| **Key phrase** | *Policy in Git, not in Confluence* | *Least privilege per intent, not per identity* | *With lineage: 90 seconds. Without: 3 weeks.* | *Who governs the governor?* |

---

## What's in this repo

| File | What it is |
|---|---|
| [`DataGovOps DES 2026 (Session Info).pdf`](./DataGovOps%20DES%202026%20(Session%20Info).pdf) | Session brief — purpose, audience fit, session flow, and design principles |
| [`DataGovOps_Canvas.html`](./DataGovOps_Canvas.html) | Interactive DataGovOps Canvas — a diagnostic tool for assessing AI governance maturity across the four moves. Open in any browser. Print-optimized for workshops. |
| [`datagovops-canvas.skill`](./datagovops-canvas.skill) | Claude skill that guides you through populating a DataGovOps Canvas via adaptive conversation. Install in any Claude project. |
| [`DataGovOps_SKILL_MD.md`](./DataGovOps_SKILL_MD.md) | The skill definition — readable version of the conversation architecture, question bank, and output specs |

---

## Three things to do Monday morning

1. **Audit one AI pipeline end-to-end.** Trace a single user's data from source to agent output. If you can't, that's your starting point.
2. **Move one policy from a document into code.** Any policy. One policy. Build the muscle memory.
3. **Map access by intent for one high-risk AI system.** Not "who" — but "for what."

---

## The DataGovOps Canvas

The canvas is a structured diagnostic for assessing how governed your AI systems are across the four moves. It works at two levels:

- **System-level:** assess a specific AI system (a RAG bot, a code assistant, an internal agent)
- **Organization-level:** assess governance posture across your portfolio of AI systems

Open [`DataGovOps_Canvas.html`](./DataGovOps_Canvas.html) in a browser to use it interactively, or install the [`datagovops-canvas.skill`](./datagovops-canvas.skill) in Claude to have an AI-guided conversation that populates the canvas for you.

---

## Speaker

**Piyush Ahuja** · Director, Tata Digital

[LinkedIn](https://www.linkedin.com/in/piyushahuja/) · [GitHub](https://github.com/piyush-ahuja)

---

## License

This material is shared for educational and professional use. Attribution appreciated.
