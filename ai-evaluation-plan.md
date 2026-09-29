# Feintt.ai AI Evaluation Plan

## Purpose

Define how AI-assisted workflows will be evaluated before they are trusted in the product.

## AI Workflows In Scope

- News classification.
- Transfer signal classification.
- Source summarization.
- Entity linking assistance.
- Review-priority scoring.

## Evaluation Dimensions

| Dimension | Question | Example Metric |
|---|---|---|
| Accuracy | Did the AI classify the item correctly? | Classification pass rate |
| Trust | Did it separate verified facts from rumors? | False verification rate |
| Entity quality | Did it connect the right player, club, league, or match? | Entity-linking error rate |
| Usefulness | Did the output help the reviewer move faster? | Reviewer time saved |
| Safety | Did it overstate, invent, or publish sensitive claims? | Critical failure count |
| Cost | Is the workflow economically reasonable? | Cost per processed item |

## Golden Set

Create an initial golden set of 50 reviewed examples:

- Official transfer
- Rumor
- Injury update
- Squad update
- Staff change
- Match report
- Duplicate / irrelevant item

Each example should include:

- Source link
- Expected category
- Expected entities
- Acceptable summary
- Failure notes

## Go / No-Go Rule

AI output cannot bypass human review for sensitive items until quality, failure modes, and correction workflows are documented.

