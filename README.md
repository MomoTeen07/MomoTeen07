# Abdoulkarim Mohamed

**QA Automation Engineer (junior) — Python · Playwright · API testing · CI/CD**

<!-- À décommenter quand ces informations seront validées :
📍 Ville, Belgique · Ouvert aux postes QA automation junior · [CV](lien) · contact@exemple.be
-->

Je construis des **systèmes de test**, pas des catalogues de scripts : conception basée sur les
risques, automatisation API et UI, exécution en CI, et rapports qu'une équipe peut réellement exploiter.

> **Statut — deux projets publics, en cours de finalisation.**
> [`football-qa`](https://github.com/MomoTeen07/football-qa) : application support et campagne de test.
> [`football-qa-agents`](https://github.com/MomoTeen07/football-qa-agents) : orchestrateur de tests multi-agents.
> La campagne **V1 est terminée et figée** ; la **V3 est en cours**. Je préfère l'écrire ici plutôt que
> de laisser croire que tout est livré — le détail est dans chaque `docs/ROADMAP.md`.

---

## Ce que je sais faire — et où c'est vérifiable

| Compétence | Preuve dans le code |
| --- | --- |
| Conception de tests et analyse de risques (P × I) | [`TEST_PLAN.md`](https://github.com/MomoTeen07/football-qa/blob/main/docs/TEST_PLAN.md) |
| Cas de test manuels (36 exécutés en V1, 50 conçus) | [`TEST_CASES.md`](https://github.com/MomoTeen07/football-qa/blob/main/docs/TEST_CASES.md) |
| Traçabilité exigence → cas → exécution → anomalie | [`TRACEABILITY.md`](https://github.com/MomoTeen07/football-qa/blob/main/docs/TRACEABILITY.md) |
| Rapports d'anomalies (gravité, preuve, correctif proposé) | [`ANOMALIES.md`](https://github.com/MomoTeen07/football-qa/blob/main/docs/ANOMALIES.md) |
| Synthèse de campagne et risques résiduels | [`CAMPAIGN_REPORT.md`](https://github.com/MomoTeen07/football-qa/blob/main/docs/CAMPAIGN_REPORT.md) |
| Automatisation UI — Playwright, Page Object Model | [`tests/playwright/`](https://github.com/MomoTeen07/football-qa/tree/main/tests/playwright) |
| Tests de contrat API — pytest + JSON Schema | [`tests/pytest/`](https://github.com/MomoTeen07/football-qa/tree/main/tests/pytest) |
| API chaînée — Postman / Newman | [`postman/`](https://github.com/MomoTeen07/football-qa/tree/main/postman) |
| CI/CD — GitHub Actions, Docker, artefacts de test | [`ci.yml`](https://github.com/MomoTeen07/football-qa/blob/main/.github/workflows/ci.yml) |
| Sécurité — JWT falsifié, cloisonnement des comptes | [`test_security.py`](https://github.com/MomoTeen07/football-qa/blob/main/tests/pytest/tests/test_security.py) |
| Orchestration multi-agents — LangGraph, LLM | [`football-qa-agents`](https://github.com/MomoTeen07/football-qa-agents) |
| Application full-stack (support de test) | [`backend/`](https://github.com/MomoTeen07/football-qa/tree/main/backend) · [`frontend/`](https://github.com/MomoTeen07/football-qa/tree/main/frontend) |

Chaque ligne pointe vers un fichier, pas vers une déclaration.

## Projets

### [Football QA](https://github.com/MomoTeen07/football-qa) — application full-stack et campagne de test

Application FastAPI / React / PostgreSQL (18 endpoints, JWT, migrations Alembic) utilisée comme
**système sous test**, volontairement non corrigée.

- **V1 terminée et figée** : 36 cas manuels, 118 vérifications automatisées, 5 anomalies documentées
- **V3 en cours** : fonctionnalités fusionnées, campagne manuelle à mener
- Tests d'API (pytest + JSON Schema), E2E Playwright en Page Object Model, collection Postman chaînée
- CI Docker avec artefacts Allure, Playwright et Postman à chaque pull request

`Python` · `FastAPI` · `PostgreSQL` · `Playwright` · `pytest` · `Postman` · `Allure` · `Docker`

### [Football QA Agents](https://github.com/MomoTeen07/football-qa-agents) — orchestrateur de tests multi-agents

Sept agents spécialisés autour d'un manager : analyse, conception, API, UI, DevOps, reporting.
Une instruction en langage naturel déclenche une mission complète, de la planification au rapport Allure.

- Orchestration **LangGraph**, pilotage **Telegram**, exécution sur une stack isolée
- **161 tests** couvrent le système d'orchestration lui-même (store, reprise, sécurité, bureau virtuel)
- Garde-fous : cibles réseau limitées à la stack de test, secrets masqués, publication Git opt-in
- Ruff et CI sur chaque pull request, sans clé ni réseau

`Python` · `LangGraph` · `Playwright` · `Telegram` · `SQLite` · `Allure` · `Docker`

## Comment je travaille

- **Piloté par le risque** : chaque campagne commence par une analyse probabilité × impact, pas par l'écriture de scripts.
- **Honnête sur les échecs** : les anomalies sont documentées, rejouées et marquées `xfail(strict=True)` — jamais supprimées pour faire passer la CI.
- **La CI comme garde-fou** : une suite verte n'est pas un argument, c'est une condition d'entrée.

## Contact

[LinkedIn](https://www.linkedin.com/in/mohamed-abdoulkarim/) · [GitHub](https://github.com/MomoTeen07)
