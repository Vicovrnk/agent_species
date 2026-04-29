---
name: requirements-lifecycle-and-traceability
description: Governs requirements as changing assets by maintaining traceability, assessing change impact, comparing baseline vs proposed updates, supporting prioritization, and preparing approval-oriented analysis artifacts.
version: 1.0.0
metadata:
  hermes:
    category: analysis
    tags: [business-analysis, babok, requirements-lifecycle, traceability, change-impact, governance, prioritization, baselines, decision-log]
---

# Requirements Lifecycle and Traceability

## Purpose

This gene equips a species to manage requirements after they exist, treating them as governed assets rather than one-time text.

Its core behavior is to:
- maintain traceability across requirements, goals, rules, and downstream items;
- assess the impact of requirement changes;
- compare baseline vs proposed states;
- support prioritization and approval-oriented analysis;
- expose governance risks, dependency effects, and unresolved decision points.

This is a lifecycle-and-governance gene, not an upstream discovery or detailed strategy-framing gene.

## When to Use

Use this gene when the task is about:
- maintaining or analyzing an existing requirement set over time;
- understanding what a requirement change affects;
- preparing traceability views or change assessment artifacts;
- comparing a baseline requirement set with proposed changes;
- supporting approval, prioritization, or controlled requirement evolution.

Typical triggers:
- "оцени влияние изменения требований"
- "подготовь матрицу трассировки"
- "сравни baseline и proposed requirements"
- "разложи change request по затронутым требованиям и рискам"
- "assess traceability and change impact for this requirement set"

## Out of Scope

Do not use this gene as the primary path for:
- discovering stakeholders or planning elicitation;
- writing the first detailed requirement set from raw notes;
- broad current/future state strategy framing;
- evaluating post-implementation business value and KPI outcomes.

If requirements are still raw and unstable, hand off upstream to requirement structuring.
If the main need is to understand why the change exists at all, hand off to strategy analysis.

## Inputs to Gather

Before lifecycle and traceability analysis, gather as many of these as are available:
- current requirement set or backlog;
- source goals, policies, business rules, decisions, scope statements, or upstream artifacts;
- change request or proposed requirement updates;
- known dependencies, impacted teams, systems, processes, releases, or controls;
- existing priorities, baselines, or approval constraints.

## Procedure

1. Establish the governed scope.
   - Identify which requirement set, baseline, backlog slice, or change request is under analysis.
   - Clarify what decisions the lifecycle output must support.
   - Separate confirmed scope from assumed scope.

2. Build or review traceability logic.
   - Link requirements to relevant goals, business rules, constraints, actors, systems, risks, or downstream artifacts when evidence exists.
   - Keep trace links meaningful; do not create decorative links with no analytical value.
   - Call out missing lineage where it blocks confidence.

3. Assess proposed changes.
   - Compare the baseline state against proposed additions, edits, removals, or reprioritizations.
   - Identify what each change affects directly and indirectly.
   - Surface dependency shifts, sequencing issues, conflicts, and possible orphaned items.

4. Evaluate impact and governance risk.
   - Assess operational, scope, compliance, ownership, timing, and coordination impacts.
   - Distinguish high-confidence impacts from speculative ones.
   - Flag changes that require explicit approval or escalation.

5. Support prioritization and decision readiness.
   - Organize changes by business importance, dependency criticality, urgency, and risk.
   - Record rationale for why some changes should move first, wait, split, or be rejected.
   - Make unresolved decision points explicit.

6. Emit lifecycle outputs.
   - Produce traceability views, change assessments, baseline comparisons, and decision-support notes.
   - State confidence limits and missing evidence.
   - Recommend the next downstream step: approval, further requirement cleanup, or implementation planning.

## Default Outputs

This gene should usually produce one or more of:
- a traceability matrix;
- a change assessment memo;
- a baseline vs proposed comparison;
- a decision log;
- a prioritized impact view of requirement changes.

## Quality Rules

- Do not create traceability for its own sake; each link should help analysis or governance.
- Distinguish direct impact from indirect or speculative impact.
- Keep baseline and proposed states visibly separate.
- Record unknown impact areas explicitly instead of masking them.
- Keep prioritization rationale explainable and auditable.
- If approval is required, say why and by whom if known.

## Negative Examples

Bad:
- "Это изменение затрагивает все требования"
- "Нужно обновить трассировку"
- "Приоритет высокий, потому что это важно"

Better:
- "Изменение правила расчета скидки напрямую затрагивает требования R-12, R-17 и отчетную логику в блоке ежемесячной сверки; косвенно влияет на контрольные проверки, завязанные на порог скидки."
- "Трассировочный разрыв: требование R-22 связано с интерфейсным изменением, но не имеет явной связи с business goal и owner approval."
- "Изменение рекомендуется приоритизировать после обновления политики согласования, иначе требования будут утверждены на основании устаревшего правила."

## Handoff Rules

- If baseline quality is weak, hand off to requirement structuring before deep governance work.
- If the main challenge is unresolved business rationale, hand off to strategy analysis.
- If governance outputs are sufficient, hand off to approval or implementation planning rather than extending analysis unnecessarily.

## Validation Prompts

Positive:
- "Подготовь матрицу трассировки и impact analysis для change request по процессу возвратов."
- "Compare the baseline and proposed requirement sets and identify approval risks, dependencies, and reprioritization needs."

Negative:
- "Определи, каких стейкхолдеров опрашивать" — this belongs to stakeholder and elicitation design.
- "Сформулируй business need и целевое состояние" — this belongs to strategy analysis, not lifecycle governance.
