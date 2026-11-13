---
name: em-dialogue-efficiency
description: "Compatibility entry for the two-step em-dialogue workflow. When the user requests dialogue efficiency or this legacy name, run scene/character assessment followed by line-level efficiency editing rather than the old standalone scoring workflow."
---

# Emma Screenwriting · Dialogue Efficiency — Compatibility Entry

## Guided decision mode (only when requested)

Enable this mode when the user says “walk me through this,” “help me think,” “ask me first,” or explicitly requests questions before drafting. Otherwise, carry out ordinary writing, analysis, and revision requests directly. This mode overrides default continuous execution or fixed questionnaires. Pass it through the main router, compatibility entries, and downstream modules without restarting intake.

1. Read the current material and valid context first. Separate established decisions, locked elements, and genuinely unresolved choices. Do not ask questions already answered. Request only essential missing material; do not invent backstory.
2. Identify the unresolved decisions that most affect the result. Ask at most three independent key questions per round, ordered by impact. Do not hide several questions inside one, pad the count, or steer a multiple-choice question toward a predetermined answer.
3. Explain why each decision matters. When useful, offer two or three directions and explain concretely how they affect characters, relationships, plot, audience anticipation, or the requested deliverable. Allow the user's own direction. An analysis-only request does not require changing the story.
4. Wait for the answers before turning the choices into the authorized proposal. Brief examples may clarify options, but do not deliver the complete solution or decide core creative choices in advance. With partial answers, continue only work independent of the unanswered choices. Silence is not a choice.
5. Briefly restate confirmed decisions, apply them to characters, events, pacing, or the relevant output, and check downstream effects. Ask another round only if important decisions remain. If none remain, explain the existing basis and finish the step without inventing questions.
6. If the user delegates judgment (“you decide”), proceed within that scope while preserving locked elements. Apply the choices to this project, not as automatic rules for other projects.

Starter: “Use [skill name] to walk me through this step. Read my material first and identify the creative decisions that will most affect the result but that I haven't made yet. Ask at most three key questions per round and explain how the options would affect the characters and plot. Don't repeat questions I've already answered. Wait for my answers before developing the proposal.”

Read and execute [em-dialogue](../em-dialogue/SKILL.md). Complete Step 1 before Step 2; reuse steps already performed in the current task rather than scoring or rewriting twice. Respect one-step, diagnosis-only, or clean-draft requests.

Retain the F/E dimensions and S=max(F,E) editorial convention, with deletion below 5 and rewriting from 5 to below 7. Current `em-dialogue` governs definitions, character appeal, emotional protection, factual locks, formatting, and delivery. Historical rules must not override the current two-step method.

When maintenance is explicitly authorized, update `em-dialogue` and its `references/dialogue-principles.md`, not two conflicting rule sets. Install both directories; this compatibility entry does not contain the full method.

If `em-dialogue` is missing from the current list, search installed skills by name and read it. Do not claim to have completed the full two-step workflow from this routing page alone.
