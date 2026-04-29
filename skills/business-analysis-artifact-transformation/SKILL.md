---
name: business-analysis-artifact-transformation
description: Transforms business-analysis artifacts between formats and fidelity levels while preserving intent, separating fact from inference, exposing assumptions and compression losses, and keeping lightweight traceability from source to output.
version: 1.0.0
metadata:
  hermes:
    category: analysis
    tags: [business-analysis, artifact-transformation, summaries, decision-memos, backlog, traceability, fidelity, babok]
---

# Business Analysis Artifact Transformation

## Purpose

This gene equips a species to safely transform BA artifacts from one form into another without losing analytical integrity.

Its core behavior is to:
- declare source, target, audience, and fidelity level before transforming;
- preserve intent while changing format;
- separate facts, inferences, and recommendations;
- expose assumptions and compression losses;
- keep lightweight traceability from source material to transformed output.

This is a transformation gene, not a substitute for the primary analytical gene that originally generated the content.

## When to Use

Use this gene when the task is about:
- converting transcripts or notes into structured summaries;
- turning summaries into decision memos, action briefs, or backlog slices;
- reframing strategic material into operational or executive form;
- compressing or expanding BA artifacts for different audiences;
- preserving analytical clarity across artifact conversions.

Typical triggers:
- "преобразуй эти notes в decision memo"
- "сделай из интервью executive summary и action brief"
- "перегони strategy findings в backlog slice"
- "сожми этот BA-артефакт до управленческой версии"
- "transform this analysis artifact into a decision-ready format"

## Out of Scope

Do not use this gene as the primary path for:
- original stakeholder discovery;
- writing requirements from scratch when the inputs are still too raw;
- full document management governance;
- pretending transformed output is more certain than the source evidence.

If the source artifact is too weak or ambiguous, hand off upstream before transforming aggressively.
If the main need is prioritization or conflict resolution, hand off to the corresponding BA gene.

## Inputs to Gather

Before transforming an artifact, gather as many of these as are available:
- source artifact or source materials;
- target artifact type;
- intended audience;
- desired fidelity or compression level;
- known assumptions, unresolved issues, and decision context.

## Procedure

1. Clarify the transformation contract.
   - State the source artifact, target artifact, audience, and purpose.
   - Clarify whether the goal is summarization, normalization, conversion, compression, or re-framing.
   - State the acceptable loss tolerance.

2. Inspect source quality.
   - Distinguish strong evidence from ambiguous or partial inputs.
   - Mark contradictions, unknowns, and low-confidence areas before transformation.
   - Do not hide source weakness inside polished output.

3. Apply transformation rules.
   - Preserve the underlying intent.
   - Separate facts, inferences, and recommendations.
   - Normalize wording when useful, but do not invent missing certainty.
   - Keep transformation proportional to source quality.

4. Expose assumptions and compression losses.
   - Call out what was inferred.
   - State what detail was dropped or collapsed.
   - Mark where the transformed artifact should not be treated as a substitute for the source.

5. Emit traceable output.
   - Produce the target artifact in a clear structure.
   - Maintain a lightweight source-to-output mapping when the risk of distortion is non-trivial.
   - Recommend whether the output is ready for decisions, backlog shaping, or further analysis.

## Default Outputs

This gene should usually produce one or more of:
- a transformation spec;
- an artifact conversion map;
- a compression ladder;
- an executive summary;
- an action brief.

## Quality Rules

- Do not hide uncertainty through formatting.
- Preserve intent even when changing structure.
- Separate observation from interpretation.
- Mark assumptions and dropped detail explicitly when they matter.
- Match fidelity to audience and decision need.
- If the transformation is lossy, say so.

## Negative Examples

Bad:
- "Я просто сократил документ"
- "В summary попали только удобные выводы"
- "Decision memo выглядит уверенно, хотя исходные данные спорные"

Better:
- "Из исходного интервью были выделены подтвержденные pain points, отдельно отмечены inferred risks и два unresolved contradictions, которые не должны исчезнуть в executive summary."
- "Стратегический memo преобразован в backlog-oriented brief с сохранением ключевых assumptions и пометкой, что приоритеты ещё не утверждены."
- "Для управленческой версии часть operational detail была опущена; это отмечено в compression notes, чтобы документ не воспринимался как полная замена исходного анализа."

## Handoff Rules

- If the transformed artifact will drive prioritization, hand off to prioritization and backlog shaping.
- If the transformed artifact reveals unresolved disagreement, hand off to stakeholder conflict and decision facilitation.
- If the transformed artifact is only a bridge between BA stages, hand off to business-analysis orchestration.

## Validation Prompts

Positive:
- "Преобразуй результаты discovery-интервью в executive summary, decision memo и action brief, явно отделяя факты от интерпретаций."
- "Transform this strategy analysis into a backlog-oriented brief with assumptions and compression notes."

Negative:
- "Собери исходные данные через интервью" — this belongs to stakeholder and elicitation design.
- "Выбери, что делать первым из 20 инициатив" — this belongs to prioritization and backlog shaping, not artifact transformation.
