---
name: business-need-and-state-modeling
description: Frames business need and strategic analysis by clarifying the problem or opportunity, modeling current and future state, surfacing assumptions, constraints, risks, and comparing change options and capability gaps.
version: 1.0.0
metadata:
  hermes:
    category: analysis
    tags: [business-analysis, babok, strategy-analysis, current-state, future-state, gap-analysis, risks, assumptions, constraints, options]
---

# Business Need and State Modeling

## Purpose

This gene equips a species to perform strategy-oriented business analysis before detailed specification begins.

Its core behavior is to:
- clarify the business need, problem, or opportunity;
- model the current state in operational terms;
- describe a desired future state;
- identify capability gaps, constraints, assumptions, and risks;
- compare options and trade-offs at a business-analysis level.

This is a strategic framing gene, not a detailed requirements-writing or lifecycle-governance gene.

## When to Use

Use this gene when the task is about:
- understanding why a change is needed before deciding what to build;
- framing a business problem or opportunity in a structured way;
- describing current state vs future state;
- identifying gaps between existing capability and desired outcome;
- preparing a decision-oriented view of options, risks, and change implications.

Typical triggers:
- "сформулируй business need по этой инициативе"
- "опиши текущее и целевое состояние процесса"
- "сделай gap analysis и варианты изменений"
- "разложи проблему бизнеса до уровня change options"
- "frame the current state, future state, and business need"

## Out of Scope

Do not use this gene as the primary path for:
- stakeholder mapping and interview design as the main deliverable;
- detailed requirement authoring and acceptance criteria drafting;
- long-term traceability and change approval governance;
- measuring KPI realization after implementation.

If discovery inputs are missing, hand off upstream to stakeholder and elicitation design.
If the work has already moved into stable requirement governance, hand off to lifecycle and traceability.

## Inputs to Gather

Before modeling the business need and states, gather as many of these as are available:
- business context, sponsor intent, pain points, goals, or market/operational triggers;
- current process descriptions, meeting notes, reports, incidents, complaints, or workflow artifacts;
- known constraints, dependencies, policies, budgets, deadlines, or regulatory limitations;
- known desired outcomes, success signals, and decision deadlines;
- any alternative approaches already being discussed.

## Procedure

1. Clarify the business need.
   - Restate the problem, opportunity, or change driver in concrete operational terms.
   - Distinguish symptom from underlying need when possible.
   - Separate evidence from assumption and political framing.

2. Model the current state.
   - Describe how the relevant process, service, or capability works today.
   - Identify actors, handoffs, bottlenecks, workarounds, exceptions, and pain points.
   - Call out where the current-state understanding is weak or contested.

3. Define the desired future state.
   - Describe what improved business behavior, capability, or outcome is expected.
   - Focus on the target operating reality, not only on a solution idea.
   - State success in observable or decision-useful terms.

4. Assess gaps and change implications.
   - Compare current vs future state to identify capability gaps.
   - Surface missing roles, process changes, system needs, policy barriers, and dependency risks.
   - Identify assumptions and constraints that shape the change.

5. Scan risks and uncertainties.
   - Identify risks related to execution, adoption, compliance, ownership, timing, data, and integration.
   - Distinguish hard constraints from uncertain concerns.
   - Mark areas where more discovery is needed before committing to a change direction.

6. Frame options and trade-offs.
   - Compare plausible change approaches at a business-analysis level.
   - Note trade-offs in cost, speed, scope, risk, operational burden, and value potential.
   - Avoid false precision when evidence is weak.

7. Emit decision-support outputs.
   - Produce a business-need summary, current-state and future-state artifacts, and option framing.
   - Include explicit assumptions, constraints, risks, and unresolved questions.
   - Recommend the next step: more discovery, requirement structuring, or governance preparation.

## Default Outputs

This gene should usually produce one or more of:
- a business need or problem statement;
- a current-state summary or canvas;
- a future-state definition or canvas;
- a capability gap assessment;
- an assumptions / constraints / risks register;
- an options and trade-offs summary.

## Quality Rules

- Do not confuse a proposed solution with the underlying business need.
- Prefer operational descriptions over abstract slogans.
- State where evidence is weak instead of over-claiming certainty.
- Keep current-state pain points tied to observable workflow or business effects.
- Keep future-state descriptions anchored in business outcomes, roles, and operating behavior.
- Surface assumptions and constraints explicitly; do not bury them inside prose.

## Negative Examples

Bad:
- "Нужно внедрить AI, чтобы стать эффективнее"
- "Текущее состояние плохое, целевое — хорошее"
- "Лучше автоматизировать процесс"

Better:
- "Сейчас заявки перераспределяются вручную между тремя командами без единого правила приоритета, что создает задержки до двух рабочих дней и высокий объем повторных эскалаций."
- "Целевое состояние требует, чтобы входящие заявки маршрутизировались по явным правилам, а владельцы процесса видели статус, SLA-риск и причину отклонения без ручного сбора данных."
- "Вариант A ускоряет запуск, но оставляет ручной контроль в критических исключениях; вариант B требует больше изменений в процессах, но снижает операционную нагрузку в долгую."

## Handoff Rules

- If the problem framing remains weak, recommend more elicitation before writing detailed requirements.
- If the business need and future state are clear enough, hand off to requirement structuring.
- If the main remaining concern is controlled change and traceability, hand off to lifecycle governance.

## Validation Prompts

Positive:
- "Сформулируй business need, текущее состояние, целевое состояние и gap analysis по инициативе автоматизации согласования счетов."
- "Analyze the current state, future state, and main trade-offs for redesigning this internal approval workflow."

Negative:
- "Напиши подробную спецификацию требований с acceptance criteria" — this belongs to requirement structuring, not strategy framing.
- "Подготовь матрицу трассировки требований" — this belongs to lifecycle and traceability, not business need modeling.
