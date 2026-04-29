---
name: requirements-structure-and-quality
description: Structures raw business inputs into clear, classified, testable requirements by decomposing requests, detecting ambiguity, checking quality, extracting rules and dependencies, and drafting acceptance-oriented wording.
version: 1.0.0
metadata:
  hermes:
    category: analysis
    tags: [business-analysis, babok, requirements, specification, quality, acceptance-criteria, ambiguity, dependencies, business-rules]
---

# Requirements Structure and Quality

## Purpose

This gene equips a species to transform raw business inputs into structured, analyzable, implementation-meaningful requirements.

Its core behavior is to:
- normalize and decompose requirement inputs;
- classify requirements by type and intent;
- detect ambiguity, incompleteness, inconsistency, and weak testability;
- extract business rules, constraints, assumptions, and dependencies;
- draft clearer, acceptance-oriented requirement wording.

This is a requirement-structuring gene, not a stakeholder discovery or solution evaluation gene.

## When to Use

Use this gene when the task is about:
- converting notes, requests, meeting outputs, tickets, or stakeholder statements into clear requirements;
- reviewing an existing requirement set for quality problems;
- separating functional, non-functional, rule-based, and constraint-based statements;
- improving requirement wording before handoff to product, design, engineering, or governance;
- exposing hidden gaps, assumptions, contradictions, or dependency risks in a requirement set.

Typical triggers:
- "преврати эти заметки в качественные требования"
- "проверь требования на ясность и полноту"
- "разложи сырой запрос на структурированный набор требований"
- "подготовь acceptance criteria"
- "review this requirement set for ambiguity and quality"

## Out of Scope

Do not use this gene as the primary path for:
- identifying stakeholders or designing elicitation sessions;
- framing business need through current/future state strategy analysis;
- maintaining long-term traceability and change governance;
- evaluating implemented solution outcomes and KPI realization.

If raw discovery is missing, hand off upstream to a stakeholder and elicitation gene.
If the task is mainly about strategy or future-state framing, hand off to a strategy-oriented gene.

## Inputs to Gather

Before structuring requirements, gather as many of these as are available:
- stakeholder notes, transcripts, tickets, issue lists, PRDs, briefs, process notes, workshop outputs;
- known business goals or success criteria;
- constraints, policies, compliance rules, technical limitations, deadlines;
- known actors, systems, data objects, workflows, triggers, exceptions;
- any existing requirement set or backlog to compare against.

## Procedure

1. Establish requirement context.
   - Restate the initiative or change area in practical terms.
   - Identify what the requirement set is supposed to support.
   - Separate known facts from assumptions or unvalidated expectations.

2. Normalize the raw inputs.
   - Break long, mixed, or vague statements into smaller requirement candidates.
   - Remove duplicates and merge equivalent statements carefully.
   - Keep source meaning intact while rewriting for clarity.

3. Classify the requirement candidates.
   - Distinguish among:
     - functional requirements;
     - non-functional requirements;
     - business rules;
     - constraints;
     - assumptions;
     - dependencies;
     - open questions.
   - Call out items that are not yet valid requirements and should remain as questions or risks.

4. Check requirement quality.
   - Inspect each candidate for:
     - clarity;
     - completeness;
     - consistency;
     - atomicity;
     - testability/verifiability;
     - relevance to the stated business goal.
   - Flag ambiguous words, hidden conditions, missing actors, undefined triggers, and vague success statements.

5. Improve wording and structure.
   - Rewrite requirements so that they describe expected behavior, conditions, or constraints clearly.
   - Draft acceptance-oriented language where it reduces ambiguity.
   - Keep business rules and constraints separate from feature desires.

6. Extract relationships and risks.
   - Identify dependencies between requirements, systems, actors, and policies.
   - Surface contradictions, sequencing assumptions, and missing prerequisite decisions.
   - Mark where further elicitation or strategy clarification is needed.

7. Emit structured outputs.
   - Produce a reviewed requirement set or requirement package.
   - Include quality findings, open questions, and unresolved risks.
   - Recommend the next downstream step: strategy clarification, lifecycle governance, or implementation handoff.

## Default Outputs

This gene should usually produce one or more of:
- a structured requirement specification;
- a classified requirement list;
- acceptance criteria drafts;
- a requirement quality review sheet;
- an open-questions / assumptions / dependency list.

## Quality Rules

- Do not pretend every business statement is already a valid requirement.
- Prefer explicit unknowns over silently filling gaps.
- Preserve traceable meaning from source inputs when rewriting.
- Keep requirements small enough to analyze, but not so fragmented that context disappears.
- Separate requirement content from rationale, risk, and assumption notes.
- If testability is weak, say what is missing to make verification possible.

## Negative Examples

Bad:
- "Система должна быть удобной"
- "Нужно улучшить отчеты"
- "Пользователь должен быстро получать информацию"

Better:
- "Менеджер продаж должен иметь возможность сформировать отчет по просроченным сделкам за выбранный период без выгрузки в Excel."
- "Система должна показывать статус обработки заявки не позднее чем через 5 секунд после изменения статуса в основном процессе."
- "Если заказ отклонен по причине лимита, оператор должен видеть конкретную причину отклонения и доступный остаток лимита."

## Handoff Rules

- If the core problem is still unclear, recommend strategy analysis before over-specifying requirements.
- If many gaps come from missing stakeholder input, hand back to elicitation.
- If the requirement set is stable and governance is now the main need, hand off to lifecycle and traceability work.

## Validation Prompts

Positive:
- "Преобразуй эти заметки после discovery в структурированный набор требований и acceptance criteria."
- "Review these requirements for ambiguity, missing constraints, and testability."

Negative:
- "Определи, кого опрашивать и как провести workshop" — this belongs upstream to stakeholder and elicitation design.
- "Оцени, дало ли внедрение решения бизнес-ценность" — this belongs to solution evaluation, not requirement structuring.
