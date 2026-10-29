# Evidence Log

Chronological record of development. Each entry is dated and linked to a member
and a commit. This log is updated throughout the project, not only at the end.

| Date | Member | Version | What was done | Files / commit hash | Verified by |
|---|---|---|---|---|---|
| 2026-10-22 | Bart | v0.1 | Created repository, folder structure, README, CHANGELOG, requirements, .gitignore | `README.md`, `CHANGELOG.md`, commit `<hash>` | All |
| 2026-10-22 | Dalila | v0.1 | Added initial evidence log and individual contributions template | `docs/evidence_log.md`, `docs/individual_contributions.md`, commit `<hash>` | Bart |
| 2026-10-23 | Mahshid | v0.2 | Implemented `models.py`, `rules.py`, `test_rules.py` | `app/`, `tests/`, commit `<hash>` | Ward |
| 2026-10-24 | Ward | v0.3 | Implemented FastAPI `/authorize`, `/health`, approval simulation, SQLite schema | `app/main.py`, `app/approval.py`, `app/db.py`, `db/schema.sql`, commit `<hash>` | Mahshid |
| 2026-10-25 | Karim | v0.4 | Prepared 30 scenarios in six categories, mock files, scenario design rationale | `scenarios/scenarios.json`, `data/mock_files/`, `docs/scenario_design.md`, commit `<hash>` | Abdourahmane |
| 2026-10-26 | Abdourahmane | v0.5 | Implemented `run_experiments.py`, ran 90 cases, produced `raw_results.csv` and logs | `run_experiments.py`, `results/raw_results.csv`, `logs/`, commit `<hash>` | Dalila |
| 2026-10-27 | Dalila | v0.6 | Implemented `analyze.py`, produced `metrics.csv` and five charts | `analysis/`, `results/metrics.csv`, `results/*.png`, commit `<hash>` | Bart |
| 2026-10-28 | Dalila | v0.7 | Wrote AI-use declaration and limitations section | `docs/ai_use_declaration.md`, `docs/limitations.md`, commit `<hash>` | Bart |
| 2026-10-30 | Bart | v1.0 | Final integration, version tag `v1.0`, Week 6 package submission | `CHANGELOG.md`, tag `v1.0`, commit `<hash>` | All |
