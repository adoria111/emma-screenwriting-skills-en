---
name: drama-dialogue-localizer
description: "Localize only Chinese short-drama dialogue into natural North American English. Use for dialogue-only translation, inserting English below Chinese lines, or preserving action while translating speech. Keep Chinese dialogue and action unchanged; resolve existing English against the Chinese source."
---

# Emma Screenwriting · Dialogue-Only Chinese-to-English Localization

## Guided decision mode (only when requested)

Enable this mode when the user says “walk me through this,” “help me think,” “ask me first,” or explicitly requests questions before drafting. Otherwise, carry out ordinary writing, analysis, and revision requests directly. This mode overrides default continuous execution or fixed questionnaires. Pass it through the main router, compatibility entries, and downstream modules without restarting intake.

1. Read the current material and valid context first. Separate established decisions, locked elements, and genuinely unresolved choices. Do not ask questions already answered. Request only essential missing material; do not invent backstory.
2. Identify the unresolved decisions that most affect the result. Ask at most three independent key questions per round, ordered by impact. Do not hide several questions inside one, pad the count, or steer a multiple-choice question toward a predetermined answer.
3. Explain why each decision matters. When useful, offer two or three directions and explain concretely how they affect characters, relationships, plot, audience anticipation, or the requested deliverable. Allow the user's own direction. An analysis-only request does not require changing the story.
4. Wait for the answers before turning the choices into the authorized proposal. Brief examples may clarify options, but do not deliver the complete solution or decide core creative choices in advance. With partial answers, continue only work independent of the unanswered choices. Silence is not a choice.
5. Briefly restate confirmed decisions, apply them to characters, events, pacing, or the relevant output, and check downstream effects. Ask another round only if important decisions remain. If none remain, explain the existing basis and finish the step without inventing questions.
6. If the user delegates judgment (“you decide”), proceed within that scope while preserving locked elements. Apply the choices to this project, not as automatic rules for other projects.

Starter: “Use [skill name] to walk me through this step. Read my material first and identify the creative decisions that will most affect the result but that I haven't made yet. Ask at most three key questions per round and explain how the options would affect the characters and plot. Don't repeat questions I've already answered. Wait for my answers before developing the proposal.”

## Purpose

Localize dialogue, not the whole script. Preserve action lines, scene headings, beats, and plot events unless the user explicitly asks otherwise.

Default target:

- Platforms: DramaBox / ReelShort / Tallflix and similar overseas vertical-drama apps.
- Audience: North American women, roughly 20-40.
- Style: fast, short, sharp, emotional, natural spoken English, aiming for high conversational authenticity (a style aim, not a measured score).

## Fixed Prompt Contract

When the user provides a Chinese script for dialogue localization, operate under this contract:

- Only process dialogue.
- Do not translate action lines.
- Do not rewrite action lines.
- Do not add plot events.
- Preserve Chinese dialogue and write the localized English dialogue on the next line.
- Do not output analysis, scene formatting, unrelated explanation, or Chinese explanation unless the user asks.

Internal process:

1. Extract every dialogue line that needs localization.
2. Understand context, relationships, conflict, emotion, and subtext for each line.
3. Preserve plot information, relationship facts, props, threats, reversals, humiliation, flirtation, and emotional turns.
4. Rewrite the English into North American vertical-drama spoken dialogue.
5. Output only the Chinese dialogue line plus its localized English line.

English dialogue requirements:

- Use natural American English, not Chinese-translated English.
- Use contractions where natural, such as don't, can't, I'm, you're.
- Prefer 1-8 words per line when the information allows it.
- Make lines short, sharp, direct, and emotionally playable.
- Give villains pressure and menace.
- Make protagonists sound like real people, not translation drafts.
- Preserve subtext in flirtation, threat, humiliation, and counterattack.
- Do not add plot.
- Do not change motivations.
- Do not change relationships.
- Do not replace key props.
- Do not state emotions already visible in the action.
- Do not use em dashes in English dialogue.
- Do not write long monologues.

Default output:

```text
[Localized Dialogue]

CHARACTER: [unchanged Chinese source dialogue]
Localized English dialogue.

CHARACTER: [unchanged Chinese source dialogue]
Localized English dialogue.
```

## Core Rule

Do not translate Chinese sentence by sentence. Translate the character intent, scene function, power move, and subtext into what an American short-drama character would actually say.

Good pattern:

```text
[Source meaning: Search for her. She must be nearby.]
She's close. Find her!
```

Avoid mechanically mirroring the Chinese structure:

```text
Search for me! She must be nearby!
```

## Source Priority

Use Chinese as the source of truth.

- If existing English conflicts with the Chinese, rewrite the English from the Chinese.
- If prior localized dialogue exists and mostly works, reuse it, but correct any mismatch against the Chinese.
- Do not sacrifice plot-critical information just to make a line shorter.

Plot-critical information includes:

- who is connected to whom, such as blood bond, fiance, family status, adoption, sworn pact
- supernatural mechanics, such as fated Luna, Alpha King, wolfsbane, Blackthorne scent, mark, secret passage
- threats, conditions, leverage, evidence, pregnancy, inheritance, titles, and vows
- named houses, titles, and key objects

## Output Formats

### Dialogue-Only

Use when the user asks for dialogue extraction or a clean dialogue list.

```text
[Localized Dialogue]

CHARACTER (context cue): [unchanged Chinese source dialogue]
Localized English dialogue.

CHARACTER: [unchanged Chinese source dialogue]
Localized English dialogue.
```

### Embedded Script

Use when the user asks to insert English into a script file.

- Keep all original script content unchanged.
- Insert the English line immediately after its matching Chinese dialogue line.
- Do not translate action lines.
- Do not add English under scene headings, action descriptions, captions, SFX, or outline paragraphs unless the user explicitly asks.
- If the file has a synopsis/outline before the actual script, insert only in the script section by default.
- If editing a real file, create a backup first unless the user explicitly says not to.

Example:

```text
**ADRIAN** [original Chinese direction and dialogue, unchanged]: [meaning gloss: He gestures to the vampire thugs to search; she must be nearby.]
She's close. Find her!
```

## Workflow

1. Identify the scope: dialogue-only output, embedded script, or both.
2. If working inside a script project and a source-of-truth pointer file exists, read it before modifying project files. If the user targets a non-true-source file, create or modify that explicit target without silently changing the true source.
3. Find the actual script body. Ignore outlines and episode summaries unless the user asks to localize them.
4. Extract dialogue lines and the minimum context needed to understand the line.
5. Localize each line from the Chinese, preserving plot facts and character intent.
6. Keep the Chinese dialogue line unchanged; place the English line directly below it.
7. Validate that every extracted dialogue line has exactly one English line and that no action lines were translated.

## Voice Guide

- **Lucien / Alpha male lead**: short, calm, controlling. Use commands and clipped statements. Avoid overexplaining.
- **Seraphina / vulnerable heroine**: natural fear, breath, confusion, and resistance. Avoid stiff literal phrasing.
- **Adrian / male villain**: entitled, cruel, possessive. Use short orders and humiliating threats.
- **Morgaine / female villain**: sweet with a knife, passive-aggressive, predatory, sometimes theatrical.
- **Vivian / evil mother figure**: shame, guilt, class contempt, family-honor pressure.
- **Vampires / thugs**: predatory and scary, not polished.

## Line-Level Rules

- Use contractions where natural: don't, can't, I'm, you're, she's.
- Prefer 1-8 words when the information allows it.
- A line may be longer when needed to preserve a blood pact, relationship, threat, or mechanism.
- Replace Chinese explanatory phrasing with playable English subtext.
- Make villain lines sharper and scarier when the scene is a hunt, threat, humiliation, or power play.
- Keep recurring fantasy terms if they are world terms: Alpha King, fated Luna, wolfsbane, House Blackthorne.
- Avoid em dashes in English dialogue.
- Avoid Chinese-translation phrasing such as "you have no qualification", "what kind of person are you", "you actually dare".

## Calibration Examples

Bracketed source-meaning lines below are English glosses of the original Chinese examples, not replacement source scripts. Preserve actual Chinese input unchanged in real work. Example character names and voices apply only when the project supports them. Check that a shortened example still retains every plot-critical source fact; never copy a sample at the expense of source fidelity.

```text
[Source meaning: Is there a blood bond between her and me?]
There's a blood bond between us?

[Source meaning: That scent... could she be the fated Luna I have searched for all these years?]
That scent... Is she my fated Luna?

[Source meaning: The woman has been poisoned with wolfsbane, but she also carries the Thorn family scent.]
She's been dosed with wolfsbane. But she smells like Blackthorne.

[Source meaning: You are only the orphan we adopted. Without the marriage blood pact your father made with the Duke, you would have died outside long ago.]
You're nothing but the orphan we took in. If your father hadn't sworn that blood pact with the Duke, you'd be dead in a ditch.

[Source meaning: Search for her. She must be nearby.]
She's close. Find her!

[Source meaning: Get out of the way, human doctor. You are blocking them.]
Move, human doctor. Let them feed.
```

## Validation Checklist

Before finishing:

- Confirm the output contains only the requested scope.
- Confirm Chinese dialogue lines remain unchanged.
- Confirm every localized dialogue line sits directly below the matching Chinese line.
- Confirm action lines were not translated.
- Confirm critical story facts were not dropped.
- Confirm English sounds speakable, not subtitle-like.
- Confirm English dialogue has no em dashes.
