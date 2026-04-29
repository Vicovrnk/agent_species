---
name: solution-evaluation-and-value-realization
description: Evaluates whether a solution delivers business value by defining evaluation criteria, linking goals and requirements to measures, assessing performance gaps and limitations, and recommending improvements.
version: 1.0.0
metadata:
  hermes:
    category: analysis
    tags: [business-analysis, babok, solution-evaluation, value-realization, metrics, kpi, limitations, recommendations, benefits]
---

# Solution Evaluation and Value Realization

## Purpose

This gene equips a species to evaluate an implemented or partially implemented solution from a business-analysis perspective.

Its core behavior is to:
- define evaluation criteria and success signals;
- connect business goals and requirements to measures;
- assess whether the solution is delivering expected outcomes;
- identify performance gaps, limitations, and likely causes;
- recommend actions that can increase value realization.

This is an evaluation gene, not an upstream elicitation or detailed requirement-authoring gene.

## When to Use

Use this gene when the task is about:
- evaluating whether a solution, process change, or capability is working as intended;
- defining how success should be measured after or during implementation;
- linking KPIs, outcomes, and requirements into an evaluation view;
- diagnosing limitations, shortfalls, or low-value realization;
- producing recommendation-oriented analysis for improvement.

Typical triggers:
- "оцени, дает ли решение ожидаемую бизнес-ценность"
- "свяжи KPI с требованиями и проверь performance gaps"
- "подготовь evaluation scorecard"
- "проанализируй ограничения решения и дай рекомендации"
- "evaluate whether this solution is delivering expected outcomes"

## Out of Scope

Do not use this gene as the primary path for:
- identifying stakeholders and planning discovery;
- writing the original detailed requirement set;
- governing traceability and change approval over time;
- framing the initial business need before the change is defined.

If the intended outcomes are still unclear, hand off upstream to strategy analysis.
If requirements are still unstable, hand off to requirement structuring or lifecycle governance first.

## Inputs to Gather

Before solution evaluation, gather as many of these as are available:
- business goals, expected outcomes, success criteria, or sponsor expectations;
- baseline requirement set, scope, or change rationale;
- available KPIs, measures, reports, incidents, feedback, operational metrics, or qualitative evidence;
- known limitations, complaints, adoption issues, exception cases, or workarounds;
- evaluation timing constraints and decision needs.

## Procedure

1. Clarify the evaluation target.
   - Define what solution, process change, or capability is being evaluated.
   - State what success is supposed to look like in business terms.
   - Distinguish intended outcomes from assumed outcomes.

2. Define or normalize evaluation criteria.
   - Identify which measures, indicators, or observations meaningfully reflect value.
   - Connect goals, requirements, or expected behaviors to measurable or observable outcomes.
   - Note where evaluation is limited by missing data or weak baseline definition.

3. Assess actual performance.
   - Review available evidence: metrics, incidents, user feedback, operational behavior, exception patterns, and qualitative signals.
   - Compare actual outcomes against expected outcomes.
   - Distinguish direct evidence from interpretation.

4. Identify limitations and gaps.
   - Surface performance shortfalls, adoption barriers, workflow friction, control weaknesses, and hidden operational costs.
   - Distinguish between solution limitations, process limitations, and measurement limitations.
   - Call out where the solution may technically function but still underdeliver business value.

5. Diagnose likely causes.
   - Assess whether gaps come from weak requirements, poor adoption, process mismatch, missing controls, unrealistic expectations, or incomplete implementation.
   - Avoid false certainty if evidence is partial.
   - Keep causal hypotheses explicit and reviewable.

6. Recommend value-improving actions.
   - Propose actions that can increase value realization, reduce limitations, or improve measurement quality.
   - Separate quick wins from structural fixes.
   - Make trade-offs and dependencies explicit.

7. Emit evaluation outputs.
   - Produce an evaluation plan, scorecard, benefits view, or recommendation memo as needed.
   - State confidence limits, missing measures, and unresolved questions.
   - Recommend the next downstream step: further evaluation, requirement revision, governance update, or implementation action.

## Default Outputs

This gene should usually produce one or more of:
- a solution evaluation plan;
- a scorecard of expected vs actual outcomes;
- a benefits or KPI tracking view;
- a limitations analysis;
- an improvement recommendation memo.

## Quality Rules

- Do not evaluate value using metrics that are unrelated to the original business need.
- Distinguish business value shortfall from mere feature incompleteness.
- Separate measurement gaps from solution gaps.
- Name confidence limits when evidence is weak or delayed.
- Prefer actionable recommendations over generic judgments like good or bad.
- If outcomes are mixed, say what is working and what is not.

## Negative Examples

Bad:
- "Решение не сработало"
- "Надо улучшить KPI"
- "Пользователи недовольны, значит проект неудачный"

Better:
- "Автоматизация сократила время первичной обработки, но не снизила число повторных эскалаций, потому что исключения по-прежнему обрабатываются вручную без явного владельца."
- "Целевой KPI по скорости достигнут, но ценность ограничена тем, что операционные менеджеры не видят причину блокировки заявки и продолжают делать ручные обходы."
- "Основное ограничение оценки: нет базового замера по доле повторной обработки до внедрения, поэтому эффект на rework пока подтверждается только качественными наблюдениями."

## Handoff Rules

- If expected outcomes are poorly defined, hand off to strategy analysis before claiming evaluation certainty.
- If the main problem is unstable or weak requirements, hand off to requirement structuring or lifecycle governance.
- If evaluation is strong enough, hand off to implementation improvement planning or controlled requirement updates.

## Validation Prompts

Positive:
- "Оцени, дало ли внедрение нового процесса согласования ожидаемую ценность, свяжи KPI с требованиями и дай рекомендации."
- "Create an evaluation scorecard for this process redesign and identify value gaps, limitations, and likely causes."

Negative:
- "Подготовь план интервью со стейкхолдерами" — this belongs to stakeholder and elicitation design.
- "Разложи сырые заметки в структурированный набор требований" — this belongs to requirement structuring, not solution evaluation.
