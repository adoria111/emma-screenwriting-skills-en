---
name: em-story-architect
description: "Develop an idea or approved adaptation into a core outline, character dossiers, and episode outlines, applying hook, pacing, conflict, emotional-escalation, and character-design rules."
---

# Emma Screenwriting · Story Architect

## Guided decision mode (only when requested)

Enable this mode when the user says “walk me through this,” “help me think,” “ask me first,” or explicitly requests questions before drafting. Otherwise, carry out ordinary writing, analysis, and revision requests directly. This mode overrides default continuous execution or fixed questionnaires. Pass it through the main router, compatibility entries, and downstream modules without restarting intake.

1. Read the current material and valid context first. Separate established decisions, locked elements, and genuinely unresolved choices. Do not ask questions already answered. Request only essential missing material; do not invent backstory.
2. Identify the unresolved decisions that most affect the result. Ask at most three independent key questions per round, ordered by impact. Do not hide several questions inside one, pad the count, or steer a multiple-choice question toward a predetermined answer.
3. Explain why each decision matters. When useful, offer two or three directions and explain concretely how they affect characters, relationships, plot, audience anticipation, or the requested deliverable. Allow the user's own direction. An analysis-only request does not require changing the story.
4. Wait for the answers before turning the choices into the authorized proposal. Brief examples may clarify options, but do not deliver the complete solution or decide core creative choices in advance. With partial answers, continue only work independent of the unanswered choices. Silence is not a choice.
5. Briefly restate confirmed decisions, apply them to characters, events, pacing, or the relevant output, and check downstream effects. Ask another round only if important decisions remain. If none remain, explain the existing basis and finish the step without inventing questions.
6. If the user delegates judgment (“you decide”), proceed within that scope while preserving locked elements. Apply the choices to this project, not as automatic rules for other projects.

Starter: “Use [skill name] to walk me through this step. Read my material first and identify the creative decisions that will most affect the result but that I haven't made yet. Ask at most three key questions per round and explain how the options would affect the characters and plot. Don't repeat questions I've already answered. Wait for my answers before developing the proposal.”

Public standalone adaptation of historical role `02-story-architect`. Keep its identity distinct from `em-ai-story` and `em-ai-script`; do not overwrite those installations.

Develop the user's idea, approved adaptation, or existing story into actionable outlines and characters. Inherit platform, audience, genre, and production mode; market research and AI production are not assumed.

## Read first

Read the [story architecture rules](references/writing-rules.md): phase/paywall design, emotional escalation, rhythm, conflict, opening hooks, and character development. The module works independently of the old showrunner or a preceding market-analysis step.

## Method

1. Establish scope, episode count/duration, character goals, allowed changes, and immutable facts. Reuse existing outlines/choices; ask only about substantive gaps.
2. Connect opening predicament, escalating pressure, core turns, final choice, and consequences in a core outline. The source's 500–600 Chinese-character compact-pitch example is not an English word-count requirement; adjust to the task.
3. Build character dossiers: identity, goal, deeper motive, obstacle, relationships, arc, and production-relevant visual anchors. Give antagonists concrete interests and reasons to act, not only a humiliation function.
4. Divide major events into episode actions/consequences. Track viewer/character knowledge, new developments, hook origin, and payoff timing. Protect locked reveal episodes.
5. Read continuously for motivation, causality, escalation, knowledge boundaries, and continuation; do not repeat the same argument in new locations. Keep repairs within adaptation scope.

## Delivery

Deliver the requested core outline, dossiers, and complete episode range. Suggested fields: episode, opening continuation, core event, choice, changed state, viewer/character knowledge, ending hook, and next payoff. Outline-only requests do not include scripts; full-series requests cannot stop after ten episodes.

Distinguish reference facts from new invention. Make allowed/forbidden disclosures auditable and character choices consequential.

## Public-edition boundaries

This is an independently usable public adaptation of the historical workflow. Episode counts, character/word limits, seconds, three/six-layer push-pull patterns, and reversal frequencies are genre-specific reference examples, not substitutes for the current brief, locked plot, or actual platform requirements.

- Establish region, audience, genre, language, total episodes, duration, and production mode from current context; do not default to North American female audiences or AI production.
- Complete the requested scope continuously. “First paywall block first” is a submission strategy, not an automatic stop. Pause at sample/approval points only when requested. Contracts, payment, and a fixed team are not prerequisites.
- Analysis, proposal, and actual revision are distinct permissions. Preserve established plot, characters, motives, knowledge order, and endings. Create freely only within unlocked/authorized dimensions.
- Old drafts, examples, and reference instructions do not automatically govern the current task. Pause affected work for substantive source conflicts; filenames/timestamps alone do not settle them.
- Brief playable parentheticals are allowed. Write consequential actions and performance information without forcing pupils, fists, or knuckles into every line. Place `Characters: ...` after each scene heading. Merge uninterrupted speech while preserving real actions and VO/OS distinctions.
- AI visual advice is a production-risk checklist, not a permanent claim about a model's capabilities. Test the actual version and use shot splitting/compositing where needed. Text, fine actions, and complex groups are not permanently banned.
- Examples illustrate methods; do not pass them off as original finished scenes. No payment, acceptance, or market-performance guarantee is made.
