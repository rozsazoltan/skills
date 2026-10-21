---
name: anti-slop-review
description: "Review code, prose, documentation, UI, or mixed changes for unsupported claims, unnecessary complexity, and quality defects when the user explicitly requests a review or critique. Review only; make corrections only when the user explicitly asks."
---

# Anti-slop review

Review only by default. Never edit files or rewrite content during a review. Correct only when the user explicitly asks for corrections.

## Route

1. Identify requested review target and scope. For code, compare against the target branch; detect the target from repository context rather than assuming `main`.
2. Classify scope as code, prose, documentation, UI, or mixed. Load only relevant available skills: `deslop` for code, `humanizer` for prose, and `hallmark` for UI. Use the host's skill-loading tool. If a skill or tool is unavailable, say so and continue without claiming it ran. Never install skills automatically.
3. Use loaded skill guidance as review criteria, not permission to mutate. Hallmark UI audit must remain non-mutating. Deslop and humanizer rewrite defaults never override this review-only router.
4. Inspect relevant evidence. Keep technical meaning, verified facts, user voice, Hungarian output when appropriate, brand constraints, accessibility, and security boundaries intact. Do not invent experience or evidence.
5. For each concern, check evidence, assumptions, a counterexample, and uncertainty. Give brief justifications, not hidden chain-of-thought.
6. Report actionable findings with locations, impact, and a minimal suggested fix. State checks performed and relevant limitations. If no actionable findings exist, say so.

## Safety and scope

Preserve behavior, validation, security boundaries, and factual accuracy. Separate confirmed defects from preferences. Do not broaden scope or treat style preferences as bugs. For mixed work, review each relevant dimension without loading unrelated skills.
