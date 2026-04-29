---
name: stakeholder-and-elicitation-design
description: Designs stakeholder analysis and elicitation workflows for business-analysis tasks: identifies relevant actors, plans information gathering, structures interviews or workshops, and captures clarifications for downstream requirements and strategy work.
version: 1.0.0
metadata:
  hermes:
    category: analysis
    tags: [business-analysis, babok, stakeholders, elicitation, interviews, workshops, clarification, discovery, requirements-inputs]
---

# Stakeholder and Elicitation Design

## Purpose

This gene equips a species to structure early business-analysis discovery work before detailed requirements or solution design begin.

Its core behavior is to:
- identify who matters around a change or initiative;
- map stakeholder roles, influence, needs, risks, and unknowns;
- design an elicitation approach suited to the context;
- prepare interviews, workshops, or question sets;
- capture clarifications, assumptions, contradictions, and open questions in a form that downstream analysis can use.

This is a discovery-and-collaboration gene, not a full requirements or strategy gene.

## When to Use

Use this gene when the task is about:
- understanding which stakeholders matter to a product, process, service, project, or change initiative;
- planning how to gather reliable business inputs before writing requirements;
- preparing stakeholder interviews, workshops, surveys, or structured question sets;
- turning vague business context into a clarified information backlog;
- exposing ambiguity, hidden assumptions, missing owners, or conflicting expectations early.

Typical triggers:
- "помоги определить стейкхолдеров и что у них нужно выяснить"
- "подготовь план интервью для бизнес-анализа"
- "собери вопросы для discovery-сессии"
- "структурируй, у кого что спросить перед формализацией требований"
- "design the elicitation plan for this initiative"

## Out of Scope

Do not use this gene as the primary path for:
- writing detailed requirement specifications as the main deliverable;
- deep current/future state strategy analysis;
- maintaining requirement traceability or change control;
- evaluating implemented solutions and KPI outcomes;
- generic facilitation detached from business-analysis discovery.

If the main need is requirement quality or specification, hand off to a requirements-focused gene.
If the main need is strategic problem framing, hand off to a strategy-focused gene.

## Inputs to Gather

Before designing the stakeholder and elicitation approach, gather as many of these as are available:
- initiative, problem, or change description;
- known business goals or desired outcomes;
- current artifacts: brief, PRD, process notes, tickets, meeting notes, customer complaints, internal docs;
- known teams, owners, users, operators, decision-makers, and affected groups;
- constraints on time, access, compliance, sensitivity, or language;
- what decisions the downstream analysis needs to support.

## Procedure

1. Clarify the analysis target.
   - Restate the initiative, problem, or change in operational terms.
   - Identify what must be learned before requirements or solution decisions can be trusted.
   - Separate known facts from assumptions and rumors.

2. Identify and segment stakeholders.
   - List direct users, operators, decision-makers, sponsors, implementers, support roles, governance roles, and indirectly affected groups.
   - For each stakeholder or stakeholder group, estimate:
     - relevance to the change;
     - influence over decisions;
     - expected knowledge contribution;
     - likely concerns, incentives, or resistance;
     - missing information about them.
   - Call out critical missing stakeholders instead of pretending coverage is complete.

3. Define elicitation objectives.
   - Decide what information must be extracted from each stakeholder segment.
   - Frame discovery goals such as:
     - business pain points;
     - workflow reality;
     - constraints and policies;
     - success criteria;
     - decision rules;
     - data or integration needs;
     - unresolved conflicts.
   - Convert broad goals into answerable question themes.

4. Choose the elicitation mode.
   - Select interviews, workshops, document review, observation, surveys, or asynchronous clarification based on:
     - stakeholder availability;
     - sensitivity of the topic;
     - need for alignment vs deep individual detail;
     - uncertainty level;
     - time constraints.
   - Explain why the selected mode fits better than obvious alternatives.

5. Design the session or question structure.
   - Prepare a sequenced interview guide, workshop agenda, or question pack.
   - Start from context and goals, then move into workflow, pain points, exceptions, constraints, priorities, and validation.
   - Include probes that surface:
     - hidden assumptions;
     - contradictions between actors;
     - missing ownership;
     - ambiguous terminology;
     - edge cases and exceptions.

6. Prepare capture and follow-up structure.
   - Define how findings will be recorded: facts, assumptions, risks, decisions, open questions, contradictions, and follow-ups.
   - Keep evidence separate from interpretation.
   - Track unresolved items so later requirement work does not silently inherit ambiguity.

7. Emit discovery-ready outputs.
   - Produce stakeholder map/register, elicitation plan, and interview/workshop/question artifacts.
   - State confidence limits and what still needs access or confirmation.
   - Recommend the next downstream BA step: strategy framing, requirements work, or both.

## Default Outputs

This gene should usually produce one or more of:
- a stakeholder register or stakeholder map;
- an elicitation plan;
- an interview guide, workshop plan, or structured question list;
- a clarification log with open questions and contradictions;
- a short note on discovery risks and confidence limits.

## Quality Rules

- Separate `observed or evidenced` from `assumed or inferred`.
- Do not invent stakeholders just to make the map look complete.
- Prefer explicit unknowns over false certainty.
- Questions should reveal decisions, constraints, workflows, and success criteria — not just collect opinions.
- Ask in ways that reduce ambiguity and surface conflicts early.
- Keep outputs usable by downstream requirements or strategy work without a second translation pass.

## Negative Examples

Bad:
- "Поговорить с пользователями и узнать требования"
- "Сделать список заинтересованных сторон"
- "Провести discovery"

Better:
- "Определи ключевые группы: заказчик, оператор процесса, владелец данных, исполнитель и служба поддержки; для каждой укажи цель интервью, ожидаемый вклад, риски и пробелы покрытия."
- "Подготовь интервью-гайд для операционного менеджера, чтобы выявить фактический workflow, исключения, SLA-ограничения и ручные обходы."
- "Собери журнал уточнений, где отдельно отмечены факты, предположения, противоречия и вопросы без владельца."

## Handoff Rules

- If the initiative is still poorly framed, recommend strategy analysis before detailed requirements.
- If discovery outputs are strong enough, hand off to a requirements-focused gene for normalization and quality control.
- If stakeholder conflict or missing ownership blocks progress, say so explicitly rather than manufacturing consensus.

## Validation Prompts

Positive:
- "Определи стейкхолдеров для инициативы по автоматизации закупок и подготовь план интервью по ролям."
- "Design a stakeholder map and elicitation plan for a service desk process redesign."

Negative:
- "Напиши финальную спецификацию требований" — out of scope; this gene can prepare inputs, not replace requirements structuring.
- "Оцени KPI внедрённого решения" — this belongs to solution evaluation, not elicitation design.
