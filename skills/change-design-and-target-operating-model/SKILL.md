---
name: change-design-and-target-operating-model
description: Designs the business-side shape of change by turning future-state intent into target operating model slices, process redesign views, transition options, and role, control, and information impacts without collapsing into detailed technical solution design.
version: 1.0.0
metadata:
  hermes:
    category: analysis
    tags: [business-analysis, change-design, target-operating-model, process-redesign, transition, operating-model, babok]
---

# Change Design and Target Operating Model

## Purpose

This gene equips a species to design the business-side form of change between strategy and detailed delivery.

Its core behavior is to:
- turn future-state intent into target operating model slices;
- frame process and service redesign at the business level;
- compare transition options;
- surface role, control, and information-flow implications;
- produce design-ready business change artifacts without sliding into low-level technical architecture.

This is a bridge gene between strategy and delivery, not a detailed implementation-design gene.

## When to Use

Use this gene when the task is about:
- converting strategic future-state intent into a structured business change shape;
- designing how roles, processes, controls, and information should operate after change;
- comparing transition paths from current state to target state;
- describing operating-model implications before detailed technical solutioning;
- preparing a business-side change blueprint for downstream specification or execution.

Typical triggers:
- "спроектируй целевую operating model для изменения"
- "разложи future state в process and role design"
- "сравни transition options между текущим и целевым состоянием"
- "подготовь business-side blueprint изменения"
- "design the target operating model for this business change"

## Out of Scope

Do not use this gene as the primary path for:
- initial problem framing or current-state diagnosis from scratch;
- detailed requirement specification;
- technical architecture design;
- delivery scheduling or rollout management.

If the future-state intent is still unclear, hand off upstream to business need and state modeling.
If the work has moved into detailed requirements, hand off to requirement structuring.

## Inputs to Gather

Before designing the change shape, gather as many of these as are available:
- business need and future-state intent;
- current-state findings and capability gaps;
- known business constraints, controls, ownership rules, and dependencies;
- candidate change options or transition approaches;
- known delivery boundaries and technical constraints at a high level.

## Procedure

1. Clarify the change intent.
   - Restate the future-state objective in business-operating terms.
   - Identify which business capability, process, service, or operating area is changing.
   - Separate target outcomes from premature solution assumptions.

2. Define target operating model slices.
   - Describe the target roles, handoffs, decisions, controls, information visibility, and service behavior.
   - Keep the model concrete enough for downstream design without over-specifying implementation.
   - Note areas where multiple target patterns remain viable.

3. Frame process and control redesign.
   - Identify how the target process should differ from the current one.
   - Surface implications for ownership, approvals, escalation, exceptions, and control points.
   - Keep business design principles explicit.

4. Compare transition options.
   - Evaluate plausible routes from current state to target state.
   - Compare them by disruption, coordination burden, control risk, learning speed, and reversibility.
   - Avoid treating a single path as inevitable when alternatives are still viable.

5. Map business impacts.
   - Surface role changes, operating burdens, information needs, control implications, and sequencing dependencies.
   - Distinguish target-state design from transition-state pain.
   - Identify where further requirement detailing or orchestration is needed.

6. Emit design-ready outputs.
   - Produce a target operating model canvas, process redesign sheet, transition option map, or impact map.
   - Recommend the next downstream step: requirement structuring, orchestration, or prioritization.
   - Keep the output useful for controlled change, not just inspirational.

## Default Outputs

This gene should usually produce one or more of:
- a target operating model canvas;
- a process redesign sheet;
- a transition option map;
- a role and control impact map;
- a design principles sheet.

## Quality Rules

- Do not confuse future-state aspiration with operating design.
- Avoid premature technical architecture decisions.
- Keep ownership, controls, and information flows visible.
- Separate target-state design from transition trade-offs.
- State where multiple design paths remain open.
- Produce outputs that can feed requirements or orchestration without re-interpretation.

## Negative Examples

Bad:
- "Будет новая operating model"
- "Процесс станет эффективнее"
- "Нужно просто автоматизировать шаги"

Better:
- "В целевой operating model владелец процесса получает явную точку решения по исключениям, а операционная команда видит статус и причину блокировки без ручного запроса в соседнюю функцию."
- "Вариант перехода A снижает initial disruption, но оставляет дублирующее ручное согласование на переходный период; вариант B требует большего организационного изменения, но быстрее выводит процесс в целевую форму."
- "Целевой процесс требует переноса контрольной точки из финального этапа в ранний pre-validation, иначе ожидаемый эффект по сокращению rework не будет достигнут."

## Handoff Rules

- If target-state intent is still unstable, hand off to business need and state modeling.
- If the main next need is item selection under constraints, hand off to prioritization and backlog shaping.
- If the design is coherent and needs coordinated execution flow, hand off to business-analysis orchestration.

## Validation Prompts

Positive:
- "Спроектируй target operating model для нового процесса обработки возвратов, включая role impacts, controls и transition options."
- "Design the business-side change model between current and future state and compare transition approaches."

Negative:
- "Собери исходные stakeholder интервью" — this belongs to stakeholder and elicitation design.
- "Напиши детальные acceptance criteria по системе" — this belongs to requirement structuring, not change design.
