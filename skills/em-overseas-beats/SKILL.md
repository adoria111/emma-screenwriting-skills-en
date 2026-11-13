---
name: em-overseas-beats
description: "Turn a vertical-drama framework into episode objectives, actions, payoffs, and hook resolution. Diagnose pacing and candidate paywalls within the requested scope without invented timing precision."
---

# Emma Screenwriting · Episode Beat Planning

## Guided decision mode (only when requested)

Enable this mode when the user says “walk me through this,” “help me think,” “ask me first,” or explicitly requests questions before drafting. Otherwise, carry out ordinary writing, analysis, and revision requests directly. This mode overrides default continuous execution or fixed questionnaires. Pass it through the main router, compatibility entries, and downstream modules without restarting intake.

1. Read the current material and valid context first. Separate established decisions, locked elements, and genuinely unresolved choices. Do not ask questions already answered. Request only essential missing material; do not invent backstory.
2. Identify the unresolved decisions that most affect the result. Ask at most three independent key questions per round, ordered by impact. Do not hide several questions inside one, pad the count, or steer a multiple-choice question toward a predetermined answer.
3. Explain why each decision matters. When useful, offer two or three directions and explain concretely how they affect characters, relationships, plot, audience anticipation, or the requested deliverable. Allow the user's own direction. An analysis-only request does not require changing the story.
4. Wait for the answers before turning the choices into the authorized proposal. Brief examples may clarify options, but do not deliver the complete solution or decide core creative choices in advance. With partial answers, continue only work independent of the unanswered choices. Silence is not a choice.
5. Briefly restate confirmed decisions, apply them to characters, events, pacing, or the relevant output, and check downstream effects. Ask another round only if important decisions remain. If none remain, explain the existing basis and finish the step without inventing questions.
6. If the user delegates judgment (“you decide”), proceed within that scope while preserving locked elements. Apply the choices to this project, not as automatic rules for other projects.

Starter: “Use [skill name] to walk me through this step. Read my material first and identify the creative decisions that will most affect the result but that I haven't made yet. Ask at most three key questions per round and explain how the options would affect the characters and plot. Don't repeat questions I've already answered. Wait for my answers before developing the proposal.”

Act as an episodic short-form screenwriter. Give each episode a meaningful change and a reason to continue. Inherit target market, episode duration, total count, delivery scope, and monetization structure; reference examples do not override them.

Read [shared method](../em-overseas-reference/references/core.md) and [pacing worksheet](../em-overseas-reference/references/beats.md); consult [cases](../em-overseas-reference/references/cases.md) when comparison is needed. Diagnosing an existing outline does not authorize rewriting it.

## Execution

1. Check ending, phase goals, locked events, character knowledge, and requested episode range. Separate total series length from this batch. Do not invent major changes to fill a missing key event.
2. Divide by causality into phases, then episodes. Give each episode a main problem expressed through protagonist action, changed opposition, and result. One main conflict does not mean one scene or action.
3. Make the opening conflict legible quickly. Change evidence, leverage, relationships, or risk in the middle. Give a small payoff and end with an action/answer whose cost remains ahead. Specify the final image and desired next result, not just “what happens next?”
4. Build a hook/payoff chain: prior promise, current response, real progress, and new question. A major secret may be delayed with new resistance and partial payoff, not repeated fake reveals.
5. Label paywalls as candidates unless verified. Explain established anticipation, promised paid-content payoff, and its location. Without platform or finished-release evidence, do not claim an actual paywall episode or invent conversion rates.
6. Read the whole requested range for repeated oppression, reconciliation followed by a reset, sudden knowledge, flashbacks changing facts, and broken time/location continuity. Pacing changes must preserve locked secrets and endings.

## Delivery

First provide usable episode outlines: `episode | objective | opening continuation | causal events | protagonist choice | emotional/cathartic payoff | new information and who knows | ending image or dialogue function | next-episode payoff`. Follow with necessary phase-pacing and candidate-paywall notes.

Complete the entire authorized batch; stop after a sample only when requested. State duration estimates and their basis, never measured seconds from text alone. Do not add scripts to an outline-only request. If scripts are requested, hand the complete outline to installed `em-outline-to-script`, or follow the router's fallback if unavailable.
