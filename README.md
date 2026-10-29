# AgentWatch

**Securing Autonomous AI Agents Through Permission Controls and Human Approval**

AgentWatch is a research framework for evaluating whether combining task-based
permission checks with risk-based human approval reduces contextually inappropriate
actions by autonomous AI agents, and what effect this has on task completion efficiency.

This repository contains the prototype, the 30 controlled simulation scenarios, the
experiment runner, the evaluation scripts, and the documentation required for the
Emtec Project (Week 6 milestone onward).

---

## Project members

| Member | ID |
|---|---|
| Bart | 7922711 |
| Mahshid | 8765753 |
| Ward | 7837495 |
| Karim | 8117652 |
| Abdourahmane | 9883290 |
| Dalila | 9069227 |

---

## Purpose

Autonomous AI agents can plan actions and use tools, but they may also perform actions
that are technically authorized yet inappropriate for the task at hand. AgentWatch
compares three authorization strategies:

1. **Unrestricted execution** — no controls (baseline).
2. **Permission checks only** — allow/deny based on static permissions.
3. **Permission checks + context-aware risk assessment + human approval** — the hybrid
   model proposed in this project.

The evaluation uses 30 controlled scenarios across six categories and measures five
metrics: blocking rate, false positive rate, task success rate, approval frequency,
and task completion time.

---

## Architecture

The prototype consists of:

- **`app/rules.py`** — permission check, risk classification, context check, decision logic
- **`app/main.py`** — FastAPI endpoints (`/authorize`, `/health`)
- **`app/approval.py`** — simulated human approval
- **`app/db.py`** + **`db/schema.sql`** — SQLite storage of scenarios, decisions and results
- **`scenarios/scenarios.json`** — 30 scenarios in 6 categories (5 each)
- **`run_experiments.py`** — runs 30 scenarios × 3 strategies = 90 cases, logs to SQLite and CSV
- **`analysis/analyze.py`** — computes the 5 metrics and produces 5 comparative charts
