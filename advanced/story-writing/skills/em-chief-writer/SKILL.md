---
name: em-chief-writer
description: "Expand a valid episode outline into complete scene-by-scene scripts for the requested episode range. Includes dialogue, emotion, continuity, format, and live-action, photorealistic-AI, or animated-drama production rules."
---

# Emma Screenwriting · Chief Writer

## Guided decision mode (only when requested)

Enable this mode when the user says “walk me through this,” “help me think,” “ask me first,” or explicitly requests questions before drafting. Otherwise, carry out ordinary writing, analysis, and revision requests directly. This mode overrides default continuous execution or fixed questionnaires. Pass it through the main router, compatibility entries, and downstream modules without restarting intake.

1. Read the current material and valid context first. Separate established decisions, locked elements, and genuinely unresolved choices. Do not ask questions already answered. Request only essential missing material; do not invent backstory.
2. Identify the unresolved decisions that most affect the result. Ask at most three independent key questions per round, ordered by impact. Do not hide several questions inside one, pad the count, or steer a multiple-choice question toward a predetermined answer.
3. Explain why each decision matters. When useful, offer two or three directions and explain concretely how they affect characters, relationships, plot, audience anticipation, or the requested deliverable. Allow the user's own direction. An analysis-only request does not require changing the story.
4. Wait for the answers before turning the choices into the authorized proposal. Brief examples may clarify options, but do not deliver the complete solution or decide core creative choices in advance. With partial answers, continue only work independent of the unanswered choices. Silence is not a choice.
5. Briefly restate confirmed decisions, apply them to characters, events, pacing, or the relevant output, and check downstream effects. Ask another round only if important decisions remain. If none remain, explain the existing basis and finish the step without inventing questions.
6. If the user delegates judgment (“you decide”), proceed within that scope while preserving locked elements. Apply the choices to this project, not as automatic rules for other projects.

Starter: “Use [skill name] to walk me through this step. Read my material first and identify the creative decisions that will most affect the result but that I haven't made yet. Ask at most three key questions per round and explain how the options would affect the characters and plot. Don't repeat questions I've already answered. Wait for my answers before developing the proposal.”

Public standalone adaptation of historical role `03-chief-writer`. Keep it distinct from `em-ai-story` and `em-ai-script`; do not overwrite those installations.

Write coherent, filmable scenes with legible character intention from a valid outline. Select live-action, photorealistic AI, or animated-drama mode from the current brief. A written script is not a generated video.

## Read first

Read [chief-writer rules](references/writing-rules.md). General chapters cover hooks, dialogue, emotion, episode drafting, format, knowledge/agency, and delivery checks. Use AI visuals, photorealism, and animation style only for matching production tasks. No old showrunner, private library, or additional skill is required.

## Method

1. Establish prior-episode state, current events/endpoint, allowed/forbidden revelations, relationships, props, and injury locations from authoritative sources. Pause only work affected by substantive conflicts.
2. Organize goals, obstacles, actions, reactions, and consequences before drafting action/dialogue. Do not import next episode's turn early or use atmosphere to replace missing plot.
3. Make dialogue respond and change the situation. Check repeated function, subtext, and voice. Short speech need not repeat name cues per sentence; merge uninterrupted turns.
4. Put `Characters: ...` as the first nonblank line after every scene heading. Use brief playable performance cues and actual consequential action/choice rather than author summaries.
5. Scale detail to production. Live action prioritizes playability. AI/animation may need simple connected image beats; verify actual tool capability through testing.
6. Check likely viewer misreading scene by scene, then reread neighboring episodes for premature reveals, uncaused emotion, repeated conflict, and prop continuity. Deliver after checks pass rather than manufacturing review loops.

## Delivery

Provide clean, complete scripts for the requested episodes. Add before/after/reason only when change records are requested. Include beat/VFX counts only when genuinely useful for production handoff; a checklist does not replace script text.

Do not stop at episode one or the first paywall merely because of internal batching. Pause only at explicitly requested samples/episode approvals. Preserve locked motives, relationships, clues, and endings.

## Public-edition boundaries

This is an independently usable public adaptation of the historical workflow. Episode counts, character/word limits, seconds, three/six-layer push-pull patterns, and reversal frequencies are genre-specific reference examples, not substitutes for the current brief, locked plot, or actual platform requirements.

- Establish region, audience, genre, language, total episodes, duration, and production mode from current context; do not default to North American female audiences or AI production.
- Complete the requested scope continuously. “First paywall block first” is a submission strategy, not an automatic stop. Pause at sample/approval points only when requested. Contracts, payment, and a fixed team are not prerequisites.
- Analysis, proposal, and actual revision are distinct permissions. Preserve established plot, characters, motives, knowledge order, and endings. Create freely only within unlocked/authorized dimensions.
- Old drafts, examples, and reference instructions do not automatically govern the current task. Pause affected work for substantive source conflicts; filenames/timestamps alone do not settle them.
- Brief playable parentheticals are allowed. Write consequential actions and performance information without forcing pupils, fists, or knuckles into every line. Place `Characters: ...` after each scene heading. Merge uninterrupted speech while preserving real actions and VO/OS distinctions.
- AI visual advice is a production-risk checklist, not a permanent claim about a model's capabilities. Test the actual version and use shot splitting/compositing where needed. Text, fine actions, and complex groups are not permanently banned.
- Examples illustrate methods; do not pass them off as original finished scenes. No payment, acceptance, or market-performance guarantee is made.
