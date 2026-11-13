---
name: em-dialogue
description: "Refine Chinese-language short-drama dialogue through Step 1: scene, intention, character appeal, and viewer comprehension; Step 2: line contribution, editorial scoring, cuts, and complete revision. Use for repetition, exposition, weak motivation, bland characters, unnatural dialogue, or em-dialogue-efficiency requests. Diagnosis alone does not rewrite. Route English conversion to localization tools."
---

# Emma Screenwriting · Two-Step Dialogue Refinement

## Guided decision mode (only when requested)

Enable this mode when the user says “walk me through this,” “help me think,” “ask me first,” or explicitly requests questions before drafting. Otherwise, carry out ordinary writing, analysis, and revision requests directly. This mode overrides default continuous execution or fixed questionnaires. Pass it through the main router, compatibility entries, and downstream modules without restarting intake.

1. Read the current material and valid context first. Separate established decisions, locked elements, and genuinely unresolved choices. Do not ask questions already answered. Request only essential missing material; do not invent backstory.
2. Identify the unresolved decisions that most affect the result. Ask at most three independent key questions per round, ordered by impact. Do not hide several questions inside one, pad the count, or steer a multiple-choice question toward a predetermined answer.
3. Explain why each decision matters. When useful, offer two or three directions and explain concretely how they affect characters, relationships, plot, audience anticipation, or the requested deliverable. Allow the user's own direction. An analysis-only request does not require changing the story.
4. Wait for the answers before turning the choices into the authorized proposal. Brief examples may clarify options, but do not deliver the complete solution or decide core creative choices in advance. With partial answers, continue only work independent of the unanswered choices. Silence is not a choice.
5. Briefly restate confirmed decisions, apply them to characters, events, pacing, or the relevant output, and check downstream effects. Ask another round only if important decisions remain. If none remain, explain the existing basis and finish the step without inventing questions.
6. If the user delegates judgment (“you decide”), proceed within that scope while preserving locked elements. Apply the choices to this project, not as automatic rules for other projects.

Starter: “Use [skill name] to walk me through this step. Read my material first and identify the creative decisions that will most affect the result but that I haven't made yet. Ask at most three key questions per round and explain how the options would affect the characters and plot. Don't repeat questions I've already answered. Wait for my answers before developing the proposal.”

Aim for compelling scenes, distinct characters, legible desire, and playable dialogue. Use what the character would naturally say to pursue an intention. Make their desire and view of the other person understandable without turning a motivation summary into self-analysis.

Complete Step 1 → Step 2 continuously by default, without asking for confirmation between steps or running two duplicate workflows. Respect requests for one step, diagnosis only, or a clean draft. A clean-draft request still requires internal checks. This module's source specialization is Chinese dialogue; use `em-english-polish` for an existing English draft.

## Input and scope

- Read complete relevant scenes; establish source version, episodes, language, audience, voices, and locks. Verify an existing source pointer; use a clearly identified sole draft directly.
- Preserve events, action order, relationships, motivation, knowledge, props, clues, secrets, revelation order, emotional turns, and hooks. Dialogue-only work must not silently add scene facts. Diagnosis does not write back.
- With limited text, give local conclusions and identify gaps without inventing backstory. If scene-level problems exceed scope, offer specific recommendations and continue feasible work.
- Route whole-scene refinement to `drama-script-refiner`, event/character/relationship changes to `em-adaptation`, Chinese-to-English adaptation to `em-us-localization`, and existing English to `em-english-polish`. Carry established directness, desire, emotional destination, and voice into downstream work; natural English must not weaken them.

## Step 1: assess the scene, characters, and communication

1. Identify who wants what, how someone prevents it, current leverage, and whom the result changes. If the scene is only greetings, procedure, or exposition, name the event/scene problem. Stronger words or higher scores do not repair a missing event.
2. Use a director's and promotional-editor's eye to identify effective images already present: what action showcases the character, how the opponent reacts, and which moment is memorable or excerptable. Intensity can come from a prop, public relationship, choice, or power shift. “Big scene” does not mechanically mean extra people, fights, or expense. Dialogue-only work leaves action unchanged.
3. Set the intended character effect: affection, sympathy, admiration, anticipation, pressure, dislike, fear, or a child's specific desire/personality. Do not villainize every supporting character or turn every lead into a cold one-liner machine. Build voice from identity, experience, addressee, habitual tactics, and rhythm, not random slang/catchphrases.
4. Check specificity, purpose, and necessity: why this person says this now to this listener, what response they want, and what deletion would lose.
5. Reduce comprehension effort. Assume one hearing without pausing, replaying, or researching background. Clarify core desire, moral attitude, relationship, and cost; avoid tongue-twisters, abstractions, and reliance on cultural allusions. Nationality or schooling is not a measure of intelligence.
6. Separate viewer and character knowledge. Viewers understanding malice does not require a villain publicly confessing. Preserve flirtation, deception, identity secrets, and information gaps. Directness does not mean revealing secrets; subtext is not mandatory for every good line.
7. Allocate information among action, speech, and inner voice. Explain less when action already communicates enough. Misunderstanding, hidden judgment, memory, or a decision may need inner voice when action cannot convey it precisely. Do not turn thoughts into audible speech or ban VO.

Record essential information, intended character effects, emotional steps, secrets, and candidate problems. A few sentences suffice for a short excerpt; a long table is not mandatory.

## Step 2: assess each line, revise, and read in context

### Contribution before scoring

- Number by scene and speaking turn. Assess functionally different sentences separately; one strong line cannot protect a redundant paragraph.
- Ask whether deletion loses plot information, characterization, relationship movement, emotional experience, or performance effect. Only if none is lost is it an ineffective candidate. Then assess concision and clarity of desire.
- **F /10 (function):** net contribution to necessary information, knowledge, action, decision, leverage, relationship, consequences, or currently essential world rules.
- **E /10 (emotion):** net contribution to pressure, turn, release, affection, sympathy, aversion, intimacy, individuality, or performance. Character appeal and effective pauses count; not every line needs an external event.
- Default **S = max(F, E)**, inherited from the efficiency module. This is an editorial convention, not a scientific standard or a formula personally specified by the user. Support scores with context.
- **S < 5:** delete. **5 ≤ S < 7:** rewrite. **S ≥ 7:** preserve effective content. If a line contains unique necessary information or meaningful character/emotional value, correct the score first; do not knowingly delete useful material mechanically. “Character voice” needs evidence.
- Repetition is redundant only when information, tactic, intensity, and consequence remain unchanged. Emotional escalation, loss of control, changed relationship meaning, first resistance, or a performance peak may justify repeated wording. Louder delivery or extra exclamation marks alone do not create escalation.

### Apply the revision

1. Remove pointless greetings, procedure, biography, synonymous explanations, empty aphorisms, and translationese that weakens the character. Judge the particular character and context; Chinese cultural elements are not inherently unsophisticated.
2. Turn facts into attempts to gain, induce, humiliate, bargain, refuse, or counterattack. Each turn responds to the last and creates pressure/change for the next. Use established amounts, deadlines, identities, and costs; invent no numbers, threats, history, or powers for intensity.
3. Compress through precise colloquial language while retaining emotional steps, relationship changes, rhythm, and voice. Impose neither a one-third deletion quota nor a universal line-length limit. Do not turn everyone into clipped commands.
4. Repair adjacent responses and action continuity after cuts. Deliver the full requested revision, not merely low-scoring examples. For diagnosis only, recommend dispositions without a full replacement draft.
5. Add a parenthetical only when it changes delivery, with one dominant playable direction. Put long actions in action lines. Merge uninterrupted consecutive speech by one character into one paragraph with one name cue. Preserve real action/response breaks and vocal-mode distinctions; do not merge thoughts with spoken lines.

### Acceptance and delivery

- Read the whole scene for comprehensible desire, active exchange, and intended character effect. Explicitly flag an unresolved scene-level cause.
- Verify facts, knowledge, secrets, relationships, hooks, and action order; remove redundant action/dialogue explanation without deleting necessary emotion or appeal.
- If full scoring is requested, cover every line: `location | character | original | F | E | S | contribution evidence | disposition | revision/continuation`, with coverage and deletion/rewrite/retention counts. Ordinary revisions may show only key changes while internally checking everything. Clean-draft requests receive only the clean draft.
- Finish when substantive issues are handled, not when all lines score highly, a change quota is met, a fixed loop count passes, or “zero residue” is claimed. An effective original line may remain unchanged.

## Calibration and feedback

- Read [September 30 dialogue lesson](references/course-0930.md) for subtraction, information load, forms of address, professional voice, and inner-voice necessity.
- Read [dialogue judgment framework](references/dialogue-framework.md) for contested repetition, direct outbursts, exchanges, and performance function.
- Read [principles and calibration](references/dialogue-principles.md) for the two-step connection and boundary examples.
- Follow [format and performance cues](references/format-and-performance.md) for complete scenes, character lists, necessary parentheticals, and uninterrupted speech.
- Update reusable rules only when skill maintenance is explicitly requested. A single project note is not a universal rule. Do not store/publish private project text or claim automatic background learning.
