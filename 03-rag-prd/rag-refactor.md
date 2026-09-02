## Diagnostic Diff · Juno RAG Lab

_Working notes from Module 3 Lab 1. Do not paste over `03-rag-prd/prd.md`. That file comes from the AI PRD Builder._

**Lovable prototype:** https://lovable.dev/projects/56659f40-06b3-46f7-b225-997840557dd4

### Before - Quality Mode (no strategy)

P1 CSV export crash (cited: Reliability) 
P2 Blue nav bar refresh (cited: User Experience)
P3 Dark mode (cited: User Experience)
  
Juno guesses from generic mock priorities and has no idea of RocketShip values.

### After - Strategy Mode (with RocketShip Strategy One-Pager)

P0: CSV export crash (cites "Reliability First" strategy pillar)
P3: Not Recommended - Blue nav bar (cites "What we are NOT doing")
P3: Not Recommended - Dark mode (cites "What we are NOT doing")

Every priority now defends itself with a strategy clause + a ticket ID.

### Takeaway

> RAG transformed Juno from a guesser into an evidence-backed decision-maker. The strategy document now drives its priorities not intuition or vibes.
