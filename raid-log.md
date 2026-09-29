# Feintt.ai RAID Log

## Risks

| ID | Risk | Impact | Probability | Owner | Mitigation | Status |
|---|---|---:|---:|---|---|---|
| R1 | Data source structure changes and breaks ingestion | High | Medium | Data / Engineering | Monitor failures, document source contracts, add fallback checks | Open |
| R2 | AI classifier mislabels rumors as verified facts | High | Medium | AI / Product | Human review gate, taxonomy, sample evaluation set | Open |
| R3 | Scope expands beyond Germany alpha too early | Medium | High | Program Lead | Phase gates and explicit out-of-scope list | Open |
| R4 | Entity matching errors create misleading player profiles | High | Medium | Data | Entity review workflow and duplicate detection | Open |

## Assumptions

| ID | Assumption | Validation Method | Status |
|---|---|---|---|
| A1 | Germany is the right first market for alpha | Validate source availability and user value | In progress |
| A2 | Users value trust and source context more than volume | User interviews and alpha feedback | Open |
| A3 | AI can assist classification but not replace review | Evaluation set and review error tracking | Open |

## Issues

| ID | Issue | Owner | Next Action | Due Date | Status |
|---|---|---|---|---|---|
| I1 | Define alpha release criteria | Program Lead | Draft go/no-go checklist | TBD | Open |
| I2 | Define AI evaluation sample set | AI / Product | Create first 50-case golden set | TBD | Open |

## Dependencies

| ID | Dependency | Needed By | Owner | Status |
|---|---|---|---|---|
| D1 | Stable source inventory for Germany | Ingestion workflow | Data | Open |
| D2 | Review taxonomy | AI classifier and review queue | Product | Open |
| D3 | Production monitoring signals | Release readiness | Engineering | Open |

