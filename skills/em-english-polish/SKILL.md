---
name: em-english-polish
description: "Polish existing localized English dialogue for meaning, naturalness, playability, voice, and cross-episode consistency while preserving source-language text, action, and story facts. First-time US cultural adaptation belongs to em-us-localization."
---

# Emma Screenwriting · English Dialogue Polish

## Guided decision mode (only when requested)

Enable this mode when the user says “walk me through this,” “help me think,” “ask me first,” or explicitly requests questions before drafting. Otherwise, carry out ordinary writing, analysis, and revision requests directly. This mode overrides default continuous execution or fixed questionnaires. Pass it through the main router, compatibility entries, and downstream modules without restarting intake.

1. Read the current material and valid context first. Separate established decisions, locked elements, and genuinely unresolved choices. Do not ask questions already answered. Request only essential missing material; do not invent backstory.
2. Identify the unresolved decisions that most affect the result. Ask at most three independent key questions per round, ordered by impact. Do not hide several questions inside one, pad the count, or steer a multiple-choice question toward a predetermined answer.
3. Explain why each decision matters. When useful, offer two or three directions and explain concretely how they affect characters, relationships, plot, audience anticipation, or the requested deliverable. Allow the user's own direction. An analysis-only request does not require changing the story.
4. Wait for the answers before turning the choices into the authorized proposal. Brief examples may clarify options, but do not deliver the complete solution or decide core creative choices in advance. With partial answers, continue only work independent of the unanswered choices. Silence is not a choice.
5. Briefly restate confirmed decisions, apply them to characters, events, pacing, or the relevant output, and check downstream effects. Ask another round only if important decisions remain. If none remain, explain the existing basis and finish the step without inventing questions.
6. If the user delegates judgment (“you decide”), proceed within that scope while preserving locked elements. Apply the choices to this project, not as automatic rules for other projects.

Starter: “Use [skill name] to walk me through this step. Read my material first and identify the creative decisions that will most affect the result but that I haven't made yet. Ask at most three key questions per round and explain how the options would affect the characters and plot. Don't repeat questions I've already answered. Wait for my answers before developing the proposal.”

Act as an English short-drama dialogue editor. Polish existing English or bilingual scripts for fidelity, natural speech, playability, and consistent voices. Use `em-us-localization` for first-time Chinese-to-US adaptation. Do not redesign names, region, institutions, or culture during a dialogue polish. Use `em-dialogue` for Chinese dialogue diagnosis.

Inherit the project audience, platform, and established variety of English. A requested “9.8/10” is a style aspiration, not an acceptance threshold or infinite rewrite condition.

## Verify source and scope

- Check source version, existing source pointer, locks, voice notes, and signature lines before file edits. Use `drama-truesource` if installed; otherwise check directly. When a sole source is clear, proceed and record it if necessary. Do not settle conflicting authority by timestamps alone; pause only affected writes.
- Compare English to approved localization decisions and source meaning. Do not mechanically undo approved adaptation into literal translation. Flag conflicts with unclear authority. Without Chinese source, polish existing English but state that source fidelity cannot be verified.
- Change English dialogue only. Preserve Chinese text, action, headings, sound effects, relationships, motivation, props, clues, secrets, hooks, and reveal timing. Keep locked lines unless specifically unlocked.
- Diagnosis gives locatable findings without file changes. Authorization covers the requested episodes/scenes; routine improvements need no line-by-line or batch approval.

## Scale the workflow

Handle short excerpts directly. For long/multi-turn tasks, use existing records or optional `_localization-progress.md` and `_localization-log.md` for source version, backup, coverage, changes, and unresolved items. Avoid duplicate tracking. Batch internally until the whole requested range is finished.

1. **Lock meaning:** relationships, timing, events, choices, threats, desire, props, causality, and intensity against authoritative source/approved adaptation.
2. **Speech/playability:** use contractions, sentence length, and pauses appropriate to character. Preserve necessary information/beats. Do not impose 1–8 words, split every long sentence, or change correct lines to meet a quota.
3. **Translationese/voice:** diagnose stiff address, literal idioms, overexplaining, formal phrasing, and homogenized voices. Examples are diagnostics, not blind substitutions; verify meaning first.
4. **Repair within scope:** correct naturalness, clarity, and mistranslation from the authoritative source. Preserve and flag changes requiring story/lock decisions or unresolved setting authority; continue independent work.
5. **Across scenes:** keep address, world terminology, recalled dialogue, revelations, and callbacks consistent.
6. **Finish checks:** cover all requested scenes. Fix or flag substantive issues. Repeat checks only for new edits, failures, or unresolved concerns, not until no alternative wording exists or a fixed loop count is reached.

## Constraints and validation

- Change expression without adding unsupported judgments, motives, or outcomes. Emotional intensity is not permission to add facts.
- Match profanity to original intensity, character register, and project limits; do not append profanity to neutral information.
- Retain dashes, long sentences, or formal language when useful for character/performance unless the project explicitly forbids them.
- Anchor changes by episode, scene, and speaker; identical text can recur in different contexts, so avoid blind global replacement.
- Compare protected Chinese text, action, headings, and locked material separately before/after. Check dialogue coverage and bilingual pairing. A plain diff alone proves neither semantic nor layout correctness.
- In Markdown, use blank lines or valid hard breaks for bilingual separation. In DOCX, use distinct paragraphs or explicit breaks. Inspect actual rendering.
- Deliver the complete revision and concise coverage, protected-content comparison, voice/term checks, rendering check, and unresolved items. Follow authorized output rules and keep a recoverable backup. Without a specified output rule, make a new version rather than promoting it as authoritative.

## References

Read [loop-prompt.md](references/loop-prompt.md) for a self-contained handoff and optional progress template when continuing long work or using another available host. Do not assume a `/loop` command or background scheduler exists.

Read [faithful-colloquial-and-qc.md](references/faithful-colloquial-and-qc.md) for deeper semantic, register, and coverage diagnostics.

## Consecutive speech formatting

Merge uninterrupted consecutive speech by one character into one paragraph with one name cue. Another response, action, caption, sound effect, transition, or scene change is a real boundary; blank lines, page breaks, or changed tone labels alone are not. Check complete chains of three or more sentences.

Keep one dominant delivery cue. Consolidate whispering, coaxing, breathlessness, or aggression across one turn without repeating the name sentence by sentence. Retain meaningful physical action and emotional turns in place; real interruptions still divide the turn.

“Combine into one” means one dialogue paragraph, not a grammatically broken comma chain. Keep natural questions, sentences, and pauses. Do not lose facts, reorder material, or weaken threats/resistance.

Separate thoughts, VO, and on-camera speech according to project convention. Unless explicitly allowed otherwise, a vocal-mode change remains a boundary. Preserve bilingual paragraph correspondence. English-only authorization does not permit changing Chinese text or action to force a merge.

Before delivery, scan all adjacent same-speaker chains, including different tone labels. Apply authorized merges and rescan without crossing genuine action or vocal boundaries merely to reach “zero residue.” In diagnosis-only mode, report rather than edit.

Example: `ALEX (quietly): Give me the key. / ALEX (threatening): Don't make me take it.` becomes `ALEX (a quiet threat): Give me the key. Don't make me take it.` If someone blocks Alex between the lines, retain that action and the separate turns. This illustrative English rendering does not broaden the original task's language-editing permissions.
