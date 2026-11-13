---
name: em-us-localization
description: "Adapt a Chinese short-drama source or unlocalized literal translation into a coherent US cultural setting and English or bilingual script while preserving authorized story mechanisms and dramatic functions. Use English polish for an already established US version that only needs dialogue refinement."
---

# Emma Screenwriting · US Cultural and Script Localization

## Guided decision mode (only when requested)

Enable this mode when the user says “walk me through this,” “help me think,” “ask me first,” or explicitly requests questions before drafting. Otherwise, carry out ordinary writing, analysis, and revision requests directly. This mode overrides default continuous execution or fixed questionnaires. Pass it through the main router, compatibility entries, and downstream modules without restarting intake.

1. Read the current material and valid context first. Separate established decisions, locked elements, and genuinely unresolved choices. Do not ask questions already answered. Request only essential missing material; do not invent backstory.
2. Identify the unresolved decisions that most affect the result. Ask at most three independent key questions per round, ordered by impact. Do not hide several questions inside one, pad the count, or steer a multiple-choice question toward a predetermined answer.
3. Explain why each decision matters. When useful, offer two or three directions and explain concretely how they affect characters, relationships, plot, audience anticipation, or the requested deliverable. Allow the user's own direction. An analysis-only request does not require changing the story.
4. Wait for the answers before turning the choices into the authorized proposal. Brief examples may clarify options, but do not deliver the complete solution or decide core creative choices in advance. With partial answers, continue only work independent of the unanswered choices. Silence is not a choice.
5. Briefly restate confirmed decisions, apply them to characters, events, pacing, or the relevant output, and check downstream effects. Ask another round only if important decisions remain. If none remain, explain the existing basis and finish the step without inventing questions.
6. If the user delegates judgment (“you decide”), proceed within that scope while preserving locked elements. Apply the choices to this project, not as automatic rules for other projects.

Starter: “Use [skill name] to walk me through this step. Read my material first and identify the creative decisions that will most affect the result but that I haven't made yet. Ask at most three key questions per round and explain how the options would affect the characters and plot. Don't repeat questions I've already answered. Wait for my answers before developing the proposal.”

Turn a Chinese source or unlocalized literal draft into an understandable, playable, internally consistent US version. Cultural-localization authorization does not automatically authorize plot reconstruction. Preserve unapproved changes to causality, relationships, motives, prop capabilities, clues, secrets, knowledge order, revelations, and endings.

## Routing

- **This module:** first establish US names, geography, institutions, everyday detail, cultural context, and English expression, or deliver a full English/bilingual version.
- **`em-english-polish`:** US context and English draft already exist; only refine fidelity, speech, voices, or continuity.
- **`em-adaptation`:** change character function, core motive, relationship, major event, structure, or ending. When localization explicitly includes such changes, use adaptation methods only in the authorized dimensions.
- **Review only:** provide located findings, impact, and suggestions; do not write back.

## Localization agreement

Before project-file edits, verify source pointer, authoritative draft, and locks. Use `drama-truesource` if available, otherwise check directly. If the sole source is clear, proceed and record a missing pointer if needed. Pause only outputs affected by a substantive source conflict; timestamps do not establish authority.

Extract requested episodes/scenes, languages/files, approved adaptation, immutable facts, backgrounds/kinship/ethnicity/period/register/names, locations/amounts/institutions/communications/key props/scene functions, and established platform/format requirements.

Use reasonable context-based defaults for ordinary preferences. Ask collectively only where answers change facts, locks, target region, or key cultural choices. Complete authorized work without approvals at every internal step.

## Execution

1. **Map before drafting.** For multi-episode work record names, address, locations, currency, institutions, communication, world terms, and props. For a short excerpt, summarize mappings briefly.
2. **Preserve function.** Replacements must preserve information, choices, risks, and evidentiary ability. A voice message is not a video call; property documents are not interchangeable when their legal functions differ.
3. **Localize to character background.** American does not mean white, Californian, or brand-heavy. Plausible Chinese names, Asian-family habits, hotpot, and tea may remain. Keep names, jobs, locations, and lifestyle compatible.
4. **Verify institutions/amounts.** Legal, medical, financial, policing, platform, exchange-rate, and price facts vary by place/time. Check authoritative local sources when precision matters. If unverifiable, preserve dramatic function and flag the uncertainty; invent no institutions.
5. **Write English, not a word-for-word mirror.** Preserve facts, intent, intensity, and relationship power through character-appropriate speech, pauses, and tactics. A memorable line cannot add an unsupported judgment, threat, decision, or identity.
6. **Keep format/consistency.** Retain scene/episode numbering and requested file format. Dialogue-only tasks do not rearrange action, headings, or SFX. Locate repeated strings by speaker/scene rather than replacing globally.

Read as needed: [names](references/name-table.md), [culture/function swaps](references/culture-swap.md), [dialogue localization](references/dialogue-localization.md), and [historical case](references/case-sugar-daddy.md). The case demonstrates method; it is not an authoritative source for new projects.

## Verification and delivery

Verify actual output, not number of substitutions: all requested scenes/dialogue have a processing status; names/kinship/address/ethnicity/places/institutions/amounts/terms agree; facts, relationships, motives, props, clues, secrets, knowledge, revelations, and hooks remain intact; replacements preserve function; institutional facts have evidence or flags; English reads aloud with distinct voices and no factual drift; protected Chinese/action/headings remain unchanged; output files open and representative paragraphs/tables/pages render correctly.

For Word output, use the current document workflow and retain a recoverable source. Default to a complete new version, with a short mapping summary, coverage, verification, and genuine unresolved items. Do not automatically overwrite, promote a source version, or send externally.


## Consecutive speech formatting

Merge uninterrupted consecutive speech by one character into one paragraph with one name cue. Another response, action, caption, sound effect, transition, or scene change is a real boundary; blank lines, page breaks, or changed tone labels alone are not. Check complete chains of three or more sentences.

Keep one dominant delivery cue. Consolidate whispering, coaxing, breathlessness, or aggression across one turn without repeating the name sentence by sentence. Retain meaningful physical action and emotional turns in place; real interruptions still divide the turn.

“Combine into one” means one dialogue paragraph, not a grammatically broken comma chain. Keep natural questions, sentences, and pauses. Do not lose facts, reorder material, or weaken threats/resistance.

Separate thoughts, VO, and on-camera speech according to project convention. Unless explicitly allowed otherwise, a vocal-mode change remains a boundary. Preserve bilingual paragraph correspondence. English-only authorization does not permit changing Chinese text or action to force a merge.

Before delivery, scan all adjacent same-speaker chains, including different tone labels. Apply authorized merges and rescan without crossing genuine action or vocal boundaries merely to reach “zero residue.” In diagnosis-only mode, report rather than edit.

Example: `ALEX (quietly): Give me the key. / ALEX (threatening): Don't make me take it.` becomes `ALEX (a quiet threat): Give me the key. Don't make me take it.` If someone blocks Alex between the lines, retain that action and the separate turns. This illustrative English rendering does not broaden the original task's language-editing permissions.
