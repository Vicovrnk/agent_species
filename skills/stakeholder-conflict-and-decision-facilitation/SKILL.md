---
name: stakeholder-conflict-and-decision-facilitation
description: Facilitates stakeholder disagreement by reframing positions into interests, surfacing shared goals and non-negotiables, structuring decision criteria and options, and moving conflicts toward decision-ready outcomes with explicit dissent and escalation paths.
version: 1.0.0
metadata:
  hermes:
    category: analysis
    tags: [business-analysis, stakeholders, conflict, facilitation, decision-making, alignment, dissent, negotiation, babok]
---

# Stakeholder Conflict and Decision Facilitation

## Purpose

This gene equips a species to handle disagreement and decision friction in business-analysis work.

Its core behavior is to:
- reframe stakeholder positions into underlying interests;
- identify shared goals and non-negotiables;
- distinguish conflict on facts, goals, constraints, or risk tolerance;
- structure options and decision criteria;
- document dissent without blocking forward motion;
- prepare escalation when consensus is not possible.

This is a conflict-and-alignment gene, not a stakeholder-discovery or generic negotiation gene.

## When to Use

Use this gene when the task is about:
- conflicting stakeholder requests or incompatible preferences;
- blocked decisions caused by unclear criteria or ownership;
- facilitating alignment without pretending everyone agrees;
- turning an argument into a structured decision process;
- making dissent visible and decision-ready.

Typical triggers:
- "у нас конфликт между стейкхолдерами, помоги структурировать решение"
- "собери disagreement в decision memo"
- "помоги провести alignment без фальшивого консенсуса"
- "раздели позиции, интересы и критерии решения"
- "facilitate a decision between competing stakeholder positions"

## Out of Scope

Do not use this gene as the primary path for:
- initial stakeholder identification and elicitation planning;
- writing the detailed requirement set;
- formal legal mediation or adversarial negotiation strategy;
- delivery project management or executive authority substitution.

If stakeholder mapping is still missing, hand off upstream to stakeholder and elicitation design.
If the main task is choosing among shaped backlog items, hand off to prioritization and backlog shaping.

## Inputs to Gather

Before facilitating conflict or decision alignment, gather as many of these as are available:
- the decision that must be made;
- the stakeholder groups involved and their stated positions;
- known interests, constraints, incentives, risks, or non-negotiables;
- evidence behind competing claims;
- time constraints, escalation paths, and known decision owners.

## Procedure

1. Clarify the decision in contention.
   - State what decision is actually blocked.
   - Separate disagreement about the decision from surrounding noise.
   - Identify what happens if no decision is made.

2. Reframe positions into interests.
   - Capture what each stakeholder says they want.
   - Translate positions into underlying interests, fears, obligations, or success conditions.
   - Avoid caricaturing either side.

3. Type the conflict.
   - Distinguish whether the conflict is mainly about:
     - facts or evidence;
     - goals or priorities;
     - constraints or policies;
     - risk tolerance or timing;
     - ownership or authority.
   - This determines what kind of facilitation is needed.

4. Surface shared ground and non-negotiables.
   - Identify common goals, minimum acceptable outcomes, and hard boundaries.
   - Explicitly state where alignment already exists.
   - Keep non-negotiables separate from preferences.

5. Structure options and criteria.
   - Generate or normalize realistic options.
   - Define decision criteria before advocacy hardens further.
   - Compare options fairly against the criteria.

6. Record dissent and decision path.
   - Document unresolved disagreement honestly.
   - State what can be decided now and what requires escalation.
   - If escalation is needed, package the issue in a decision-ready form.

7. Emit facilitation outputs.
   - Produce a conflict framing sheet, decision memo, alignment tracker, or dissent log.
   - Recommend the next step: decision, escalation, more evidence gathering, or reprioritization.

## Default Outputs

This gene should usually produce one or more of:
- a conflict framing sheet;
- a decision memo;
- an alignment tracker;
- a dissent log;
- a decision criteria matrix.

## Quality Rules

- Do not confuse loud positions with core interests.
- Do not erase real conflict for the sake of harmony.
- Keep shared goals and non-negotiables explicit.
- Separate missing evidence from genuine value conflict.
- Record dissent clearly without turning it into sabotage.
- If authority boundaries matter, say who must decide rather than simulating authority.

## Negative Examples

Bad:
- "Они просто не договорились"
- "Нужно найти компромисс любой ценой"
- "Все стороны по-своему правы"

Better:
- "Команда безопасности защищает обязательный контроль доступа, а операционная команда опасается роста времени обработки. Конфликт не о цели как таковой, а о допустимом trade-off между control strictness и operational speed."
- "Стороны согласны в цели снизить ошибки согласования, но расходятся в критериях решения: для одной стороны ключевой критерий — auditability, для другой — time-to-approve."
- "Рекомендовано вынести на решение владельца процесса два варианта с явным сравнением рисков и выгоды, сохранив dissent команды эксплуатации в decision memo."

## Handoff Rules

- If the core disagreement comes from missing facts, hand off to elicitation or evidence gathering.
- If the conflict is mainly about prioritization under constraints, hand off to prioritization and backlog shaping.
- If the decision path is clear and the next need is coordinated execution, hand off to business-analysis orchestration.

## Validation Prompts

Positive:
- "Структурируй конфликт между продуктом, compliance и операциями по новому процессу онбординга и подготовь decision memo."
- "Facilitate this stakeholder disagreement, separate positions from interests, and prepare escalation-ready options."

Negative:
- "Просто составь список стейкхолдеров для инициативы" — this belongs to stakeholder and elicitation design.
- "Разложи backlog по приоритетам" — this belongs to prioritization and backlog shaping, not conflict facilitation.
