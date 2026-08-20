# AI Solution Decision Matrix · Juno

## The decision

Deciding how Juno should implement Automated Prioritization so it can synthesize scattered customer signals into evidence backed priority recommendations. This decision matters now because prioritization is a core Juno workflow, and we need to balance speed to value with control, differentiation, and implementation risk.

## Options scored

| Option | Cost | Speed | Control | Moat | Risk | Score |
|---|---|---|---|---|---|---|
| Build | 2 | 2 | 5 | 5 | 2 | 3.2 |
| Buy / API | 5 | 5 | 3 | 2 | 4 | 3.8 |
| Fine-tune | 3 | 3 | 4 | 4 | 3 | 3.4 |

## Recommendation

Buy / API is the best starting point because Juno can achieve the required RAG + Copilot capability quickly without taking on the cost and risk of building or fine-tuning a model. Juno's differentiation should come from its proprietary customer signal corpus, prioritization framework, evidence synthesis, and workflow, not from owning the underlying foundation model.
