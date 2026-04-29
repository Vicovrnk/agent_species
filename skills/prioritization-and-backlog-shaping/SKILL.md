---
name: prioritization-and-backlog-shaping
description: Shapes competing initiatives, requirements, and change items into decision-ready backlog slices by clarifying outcomes, normalizing criteria, surfacing trade-offs, and recommending sequencing under constraints.
version: 1.0.0
metadata:
  hermes:
    category: analysis
    tags: [business-analysis, prioritization, backlog, decision-making, trade-offs, sequencing, shaping, babok, value]
---

# Prioritization and Backlog Shaping

## Purpose

This gene equips a species to turn a messy set of possible work items into a decision-ready backlog.

Its core behavior is to:
- shape candidate items before scoring them;
- clarify decision scope and constraints;
- compare value, urgency, confidence, effort, and dependency risk;
- make trade-offs explicit;
- recommend sequencing such as now / next / later or ranked slices.

This is a prioritization and decision-framing gene, not a requirement-discovery or implementation-planning gene.

## When to Use

Use this gene when the task is about:
- deciding which initiatives, requirements, fixes, changes, or opportunities should move first;
- converting a raw set of ideas into shaped backlog items;
- making prioritization criteria explicit and auditable;
- comparing options under time, budget, capacity, or risk constraints;
- producing a recommended work sequence rather than only a flat list.

Typical triggers:
- "приоритизируй этот backlog"
- "помоги разложить инициативы на now / next / later"
- "сформируй backlog slice под ограниченный ресурс"
- "сравни варианты и объясни trade-offs"
- "shape and prioritize these candidate work items"

## Out of Scope

Do not use this gene as the primary path for:
- eliciting stakeholder inputs from scratch;
- writing the full detailed requirement set for each item;
- managing requirement traceability over time;
- evaluating realized value after implementation.

If item definitions are too vague, hand off upstream to discovery or requirement structuring.
If the task is mostly about delivery scheduling mechanics, hand off to a delivery-oriented workflow.

## Inputs to Gather

Before prioritizing, gather as many of these as are available:
- candidate items or opportunity list;
- business goals and strategic direction;
- constraints on time, budget, people, deadlines, or risk tolerance;
- dependencies, prerequisite decisions, compliance needs, or sequencing constraints;
- evidence on expected value, urgency, effort, confidence, or downside if delayed.

## Procedure

1. Clarify the decision frame.
   - State what is being prioritized and for what horizon.
   - Clarify whether the output should be ranked, bucketed, or sliced into phases.
   - Separate decision constraints from preferences.

2. Shape the items before scoring.
   - Normalize mixed ideas into comparable work items.
   - Split oversized items when a smaller meaningful slice exists.
   - Keep item boundaries clear enough for comparison.

3. Define or normalize criteria.
   - Use criteria such as:
     - expected value;
     - urgency or timing sensitivity;
     - confidence in the hypothesis;
     - effort or coordination burden;
     - dependency criticality;
     - risk reduction or control significance.
   - Avoid fake precision when evidence is weak.

4. Compare options and trade-offs.
   - Surface what each item optimizes and what it sacrifices.
   - Distinguish high-value but uncertain work from urgent but lower-value work.
   - Call out items that should move earlier because they unlock others.

5. Recommend backlog shape and sequence.
   - Produce a ranked list, tiered buckets, or now / next / later grouping.
   - Explain why some items are deprioritized, deferred, split, or rejected.
   - Make hidden dependency sequencing explicit.

6. Emit decision-ready output.
   - Include rationale, assumptions, and confidence limits.
   - Recommend what to do next and what not to do yet.
   - If the backlog needs re-shaping before execution, say so directly.

## Default Outputs

This gene should usually produce one or more of:
- a backlog shaping canvas;
- a prioritization table;
- a now / next / later view;
- a trade-off memo;
- a deprioritized items log with rationale.

## Quality Rules

- Do not score items that are too vague to compare honestly.
- Shape before scoring.
- Separate urgency from value.
- Make dependency-driven priority explicit.
- Prefer clear rationale over pseudo-mathematical certainty.
- If data quality is weak, mark confidence rather than pretending precision.

## Negative Examples

Bad:
- "Это важнее, потому что кажется полезным"
- "Ставим первым всё срочное"
- "Все инициативы high priority"

Better:
- "Инициатива A даёт более высокий потенциальный эффект, но зависит от ещё не подтверждённого data source; инициатива B даёт меньший upside, зато снимает текущий compliance risk и может быть реализована сразу."
- "Элемент стоит перенести в next, потому что без завершения базовой роли-ownership схемы его ценность не реализуется."
- "Элемент разделён на минимальный полезный slice и последующее расширение, чтобы не блокировать быстрый эксперимент из-за большого объёма."

## Handoff Rules

- If item definitions are still weak, hand off to discovery or requirement structuring before forcing prioritization.
- If the main blocker is stakeholder disagreement about criteria, hand off to conflict and decision facilitation.
- If prioritization is stable and the next need is orchestration, hand off to business-analysis orchestration.

## Validation Prompts

Positive:
- "Сформируй now / next / later для 12 инициатив по улучшению клиентского сервиса с учетом ограниченной capacity."
- "Shape and prioritize these candidate requirements, explain trade-offs, and identify what should be deferred."

Negative:
- "Проведи интервью со стейкхолдерами и собери исходные требования" — this belongs to stakeholder and elicitation design.
- "Оцени, сработало ли уже внедрённое решение" — this belongs to solution evaluation, not prioritization.
