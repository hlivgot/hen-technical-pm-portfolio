# Feintt.ai System Context

## Plain-English System Description

Feintt.ai collects handball information from multiple sources, structures it into product pages, uses AI-assisted workflows to classify or summarize information, and requires human review for items that may affect trust, reputation, or accuracy.

## Main Components

| Component | Purpose | TPM-Relevant Questions |
|---|---|---|
| Public web app | Shows players, clubs, leagues, news, matches, transfers, rankings | What pages must be reliable for alpha? |
| Database | Stores structured entities and workflow state | Who owns data quality and schema changes? |
| Ingestion jobs | Pull data from source pages and feeds | What happens when a source changes or fails? |
| AI classifier | Tags and summarizes incoming information | How do we evaluate accuracy and failure modes? |
| Review workflow | Lets humans approve, reject, or correct sensitive items | What must never publish automatically? |
| Monitoring | Tracks failures, quality, and readiness | What signals trigger escalation? |

## Critical Dependencies

- Source availability.
- Database schema stability.
- AI classification quality.
- Review workflow usability.
- Production deployment health.

## Technical Risks To Track

- Wrong player or club entity linked to a news item.
- Duplicate records.
- Source changes break ingestion.
- AI overstates unverified rumors.
- Production data and UI drift apart.
- No clear rollback for bad published content.

## TPM Ownership Boundary

The TPM does not need to write every technical implementation detail. The TPM must ensure that technical decisions are visible, risks are owned, dependencies are tracked, and release decisions are evidence-based.

