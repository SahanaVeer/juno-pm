# AI Strategy One-Pager - Juno Automated Prioritization

## 1. Problem & Workflow

Problem: PMs risk prioritizing and building the wrong features because they rely on rigid requirements and incomplete signals rather than understanding user intent and behavior.

Bad decision Juno prevents: Building the wrong thing for the wrong reason.

## 2. Target Metrics

Primary KPI: % of product decisions that lead to validated positive user outcomes
Target Metrics
•	Primary: Increase validated product decisions by 25% 
•	Decision quality: ≥ 80% of Juno recommendations are rated useful/actionable by PMs 
•	Efficiency: Reduce time spent on requirements/decision analysis by 30% 
•	Adoption: ≥ 70% of target PMs use Juno weekly 

## 3. Autonomy Level

Copilot: Juno augments PM judgment by analyzing signals, surfacing insights, and recommending actions while keeping the PM in control. Not Agent: We would not allow Juno to autonomously make or execute high-impact product decisions because context, tradeoffs, and business judgment still require human oversight.

## 4. Data & Model Approach

Data & Model Approach: Buy + Ground (LLM + RAG)

Use a commercially available LLM and ground its responses with Juno-specific data such as user feedback, product analytics, requirements, research, and business context through RAG. We are not taking the Fine-tune shortcut because Juno’s product context and user signals will continuously change; fine-tuning would add complexity and maintenance without being necessary for the core decision-support use case.

Shortcut we are NOT taking: Fine-tuning the model to “teach” it Juno’s context. Instead, keep the model general-purpose and retrieve the most relevant, up-to-date context at decision time.

## 5. Risks & Mitigations

Risk: Juno could confidently recommend the wrong product decision because it misinterprets user signals or lacks critical business context, leading a PM to prioritize the wrong problem.

Guardrail: Juno must show the evidence and sources behind every recommendation and require explicit PM approval before any high-impact decision is acted upon. This keeps the PM accountable and makes Juno’s reasoning auditable rather than a black-box recommendation.

## 6. V1 Scope

IN: Analyze user signals, feedback, and product context to surface patterns, identify likely user intent, and recommend product priorities or next steps.

OUT: Autonomously make or approve product decisions: the PM remains the final decision-maker.
Automatically execute changes in production:Juno will not modify features, workflows, or customer experiences without human review and approval.
