# Acceptance criteria patterns

Use acceptance-oriented wording when it reduces ambiguity.

## Useful patterns
1. Condition -> behavior -> expected result
- When [condition], the system / actor must [behavior], so that [result].

2. Given / when / then
- Given [context]
- When [action or event]
- Then [observable outcome]

3. Rule-driven outcome
- If [business rule condition], then [required outcome or restriction].

## Guidance
- Prefer observable outcomes.
- Name the actor when relevant.
- Include exceptions if they are important to correctness.
- Keep acceptance criteria aligned with the underlying requirement, not as a new hidden requirement set.
