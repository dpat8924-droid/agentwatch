# Changelog

All notable changes to the AgentWatch project are recorded in this file.
The format is based on Keep a Changelog and the project uses semantic versioning.

## [v0.1] — 2026-10-22

### Added
- Initial research proposal (`docs/proposal.md`): introduction, problem statement,
  stakeholder needs, research question, objectives, literature review and gap,
  methodology and evaluation plan, proposed solution architecture.
- Repository structure: `app/`, `scenarios/`, `analysis/`, `tests/`, `docs/`,
  `results/`, `logs/`.
- `README.md` with purpose, architecture, tools and reproduction instructions.
- `requirements.txt` and `.gitignore`.
- `docs/evidence_log.md` (initial entry).
- `docs/individual_contributions.md` (template for six members).

## [v0.2] — 2026-10-23

### Added
- `app/models.py` — data models for actions, decisions and risk levels.
- `app/rules.py` — permission check, context check, risk classification and decision logic.
- `tests/test_rules.py` — pytest tests for all six scenario categories.

## [v0.3] — 2026-10-24

### Added
- `app/main.py` — FastAPI endpoints `/authorize` and `/health`.
- `app/approval.py` — simulated human approval.
- `app/db.py` and `db/schema.sql` — SQLite schema and connection.
- `docs/screenshots/swagger.png` — screenshot of the working API.

## [v0.4] — 2026-10-25

### Added
- `scenarios/scenarios.json` — 30 scenarios in six categories (five each).
- `data/mock_files/` — fictitious documents for the simulation.
- `docs/scenario_design.md` — rationale for the six categories.

## [v0.5] — 2026-10-26

### Added
- `run_experiments.py` — runs 30 scenarios × 3 strategies = 90 cases.
- `results/raw_results.csv` — raw experiment results.
- `logs/` — run logs.

## [v0.6] — 2026-10-27

### Added
- `analysis/analyze.py` — computes five metrics and produces five charts.
- `analysis/README.md` — analysis instructions.
- `results/metrics.csv` — comparison table (3 strategies × 5 metrics).
- `results/*.png` — five comparative charts.

## [v0.7] — 2026-10-28

### Added
- `docs/ai_use_declaration.md` — GenAI and AI-assisted development declaration.
- `docs/limitations.md` — evaluation limitations, threats to validity and future work.

## [v1.0] — 2026-10-30

### Finalised
- Week 6 milestone package: repository, README, evidence log, individual contributions,
  AI-use declaration, limitations, screenshots, test evidence, results and charts.
- All six members recorded in `docs/individual_contributions.md`.
- Version tag `v1.0`.
