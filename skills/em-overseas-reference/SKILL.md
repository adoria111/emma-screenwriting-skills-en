---
name: em-overseas-reference
description: "Apply the supplied development guidelines and genre cases to concept selection, story design, episode outlines, review, and pitch packaging. Use when this reference collection is requested; single-purpose tasks should route directly to the relevant module. Not live market research or automatic submission."
---

# Emma Screenwriting · International Vertical-Drama Reference Hub

## Guided decision mode (only when requested)

Enable this mode when the user says “walk me through this,” “help me think,” “ask me first,” or explicitly requests questions before drafting. Otherwise, carry out ordinary writing, analysis, and revision requests directly. This mode overrides default continuous execution or fixed questionnaires. Pass it through the main router, compatibility entries, and downstream modules without restarting intake.

1. Read the current material and valid context first. Separate established decisions, locked elements, and genuinely unresolved choices. Do not ask questions already answered. Request only essential missing material; do not invent backstory.
2. Identify the unresolved decisions that most affect the result. Ask at most three independent key questions per round, ordered by impact. Do not hide several questions inside one, pad the count, or steer a multiple-choice question toward a predetermined answer.
3. Explain why each decision matters. When useful, offer two or three directions and explain concretely how they affect characters, relationships, plot, audience anticipation, or the requested deliverable. Allow the user's own direction. An analysis-only request does not require changing the story.
4. Wait for the answers before turning the choices into the authorized proposal. Brief examples may clarify options, but do not deliver the complete solution or decide core creative choices in advance. With partial answers, continue only work independent of the unanswered choices. Silence is not a choice.
5. Briefly restate confirmed decisions, apply them to characters, events, pacing, or the relevant output, and check downstream effects. Ask another round only if important decisions remain. If none remain, explain the existing basis and finish the step without inventing questions.
6. If the user delegates judgment (“you decide”), proceed within that scope while preserving locked elements. Apply the choices to this project, not as automatic rules for other projects.

Starter: “Use [skill name] to walk me through this step. Read my material first and identify the creative decisions that will most affect the result but that I haven't made yet. Ask at most three key questions per round and explain how the options would affect the characters and plot. Don't repeat questions I've already answered. Wait for my answers before developing the proposal.”

Act as a development editor turning audience anticipation into a sustainable story and the requested deliverable. The current agent coordinates the modules; no persistent service, fixed agent team, or stage-by-stage permission is required.

Inherit region, platform, audience, language, and live-action/AI production mode. “International” does not automatically mean North American female audiences. Work independently of missing details where possible; ask collectively only when region, core premise, or delivery scope cannot reasonably be established. Without a named platform, deliver a general development package, not purported current submission specifications.

## Establish scope

- Original work: develop within the user's goals/limits; do not rename and copy a reference's characters, dialogue, and distinctive event combination.
- Existing work: read the authoritative draft and locks; use available `drama-truesource` or equivalent direct checks before edits. Analysis or skill maintenance needs no story pointer. Pause only writes affected by substantive conflict.
- Review/proposal: deliver that output only. Module recommendations do not grant plot-change permission. Complete authorized creation/revision instead of stopping at an intermediate proposal.
- Read [method/evidence boundaries](references/core.md) on first use. Consult [source index](references/sources.md) when provenance is needed, not every original source on every task.

## Choose the smallest workflow

Read the selected module's actual SKILL.md and execute; do not merely return a command for the user to resend. Modules do not call back into this hub.

| Request | Module | Deliverable |
|---|---|---|
| Concepts, genre combinations, fit | [em-overseas-genre](../em-overseas-genre/SKILL.md) | Concept cards with tradeoffs |
| Characters, world rules, sustained conflict | [em-overseas-engine](../em-overseas-engine/SKILL.md) | Story development document |
| Episode beats, hooks, cathartic moments/payoffs | [em-overseas-beats](../em-overseas-beats/SKILL.md) | Requested outlines and payoff tracking |
| Script from a locked episode outline | Installed `em-outline-to-script` | Complete requested scenes/episodes |
| First-time US adaptation of existing material | Installed `em-us-localization` | Function-preserving localized script; an original US-set premise alone does not require this extra step |
| Readiness review against guidelines | [em-overseas-review](../em-overseas-review/SKILL.md) | Evidence-backed report |
| Submission copy, synopsis, samples | [em-overseas-pitch](../em-overseas-pitch/SKILL.md) | Reviewable package and missing items |

Typical dependency order: concept → development → episode outline → script → localization if needed → review → pitch. Start at the existing artifact's stage. A genre question does not require an entire series; a review does not authorize polish.

Reuse script/localization modules when available. Otherwise apply [writing/localization agreement](references/writing-localization.md) to feasible work and state that a missing module was not invoked. Do not impose US culture on a non-US market. Change character/event design only within scope.

## Carry decisions forward

Retain market/language, delivery scope, authoritative files, known ages, main plot, permitted changes, protected relationships/evidence, ending, production limits, and facts to verify. For short tasks, context suffices. For long projects, use one `_international-drama-status.md` with artifact paths, actual completed episodes, unresolved items, and next step; invent no progress.

At every stage check: **what the protagonist wants → who can stop them and why → action → cost/change → payoff delivered → remaining anticipation**. Genre tags, reversal counts, and sensational images cannot replace this chain.

## Deliver and finish

Provide the requested artifact with necessary coverage/uncertainty notes. Default to Markdown; use available file workflows for requested Word/PDF. Finish the authorized step and necessary checks without subjective high-score loops. Real blockers affect only dependent work. Preparing a submission does not include sending, uploading, payment, or external commitments.

Examples:
- “Use $em-overseas-reference to propose three low-budget fantasy family dramas for North American women; choose one and outline episodes 1–10.”
- “Use these guidelines to review episodes 1–8. Report problems only; do not revise.”
- “Expand the approved outline into episodes 1–5 in the requested language, preserving characters and endings.”
- “Prepare a submission package from this project. Do not send it.”
