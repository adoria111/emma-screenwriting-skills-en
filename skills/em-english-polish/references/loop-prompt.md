# Localization Review: Copy-Ready Task, Diagnostics, Templates

Read for a long-task handoff to another available host. The task block is self-contained; it is not a host-specific scheduling command and does not assume `/loop` exists.

## 1. Copy-ready task

Replace the first line with actual file paths, episode/scene range, and approved output mode.

```text
Task: Polish the already-localized English dialogue in the specified file and episodes/scenes for fidelity, natural speech, playability, and project voices. Use the target, scope, and output mode supplied with this instruction.

Verify source pointer, locks, and approved localization. Use drama-truesource if installed; otherwise verify directly. If the sole source is clear, record a missing pointer if useful and continue. Pause only writes affected by unresolved source conflicts. Existing authorization covers the complete range; do not reconfirm each batch.

Change English dialogue only. Preserve Chinese text, action, headings, SFX, and locked lines. Check approved adaptation and Chinese meaning. With English alone, improve naturalness and state that source fidelity was not verified. Do not undo approved adaptation into literal translation.

Check each scene for:
1. Facts/intent: relationships, timing, events, choices, threats, desires, props, causality, reveal timing.
2. Playable speech: character-appropriate contractions, pauses, sentence lengths without cutting facts for a quota.
3. Translationese: review meaning/register before changing address, literal idioms, stock phrases, or exposition. Do not substitute examples mechanically.
4. Voice/continuity: address, terms, recalled speech, hooks, knowledge gaps.

Apply authorized wording repairs or mistranslation corrections against the authoritative source directly. Preserve and ask precisely about new story decisions, lock overrides, or unresolved source conflicts, while continuing unaffected content.

Finish short excerpts directly. Track coverage, changes, and unresolved items only when task size/continuity benefits from a record.

After covering every requested unit, compare protected content, bilingual alignment, cross-scene consistency, and actual line rendering. Merge uninterrupted same-speaker dialogue into one paragraph with one name cue and a consolidated dominant delivery cue. Different tone labels alone do not create new turns. Preserve real action, response, and vocal-mode boundaries. Keep information/order and rescan complete chains. English-only tasks must preserve Chinese and action and maintain bilingual mapping.

Finish when substantive problems are handled or explicitly unresolved. Repeat checks only for new changes, failures, or remaining concerns, not zero alternative wording, change quotas, or subjective high scores.

Deliver the complete revised draft, coverage/validation/unresolved summary, and recoverable backup. Default to a new version without automatically promoting it as authoritative.
```

## 2. Contextual translation-artifact diagnostics

These are candidates, not universal mistakes or proof of AI authorship. See [faithful colloquialization and QC](faithful-colloquial-and-qc.md) for meaning, register, phrase checks, protected-text comparison, and version discipline.

| Candidate | Symptom | Context-sensitive response |
|---|---|---|
| Numbered sibling address | Literal “second brother” | “The middle one” only if family order and meaning support it |
| Literal idioms | Lost figurative intent | Preserve concealed danger in a “smiling tiger” metaphor; a smug pretty boy is not equivalent |
| Stated visible emotion | Speech repeats action | Remove “with jealousy” from “losing your mind with jealousy” only when motive remains clear |
| Honorific/status address | Inappropriate register | Approved name or Mr. + surname in a suitable modern setting; retain special address when world/period requires |
| Overliteral body reference | “Her legs must be exhausted” | “She must be worn out” if whole-person fatigue is intended |
| Documentary tone | “They have unusual customs” | “They've got their own ways” when register/meaning fit |
| Literal question structure | “Aren't you afraid I'm a monster?” | “You're not scared I'm a monster?” when the changed emphasis fits |
| Word-for-word mirror | “Search for me! She must be nearby!” | “She's close. Find her!” |
| Dashes | Punctuation not serving performance | Follow project convention; no universal deletion rule |
| Stock translationese | “You have no qualification,” “you actually dare” | Replace with contextual natural speech or cut redundant content |
| Premature fantasy label | “Mate” before supernatural knowledge | Use established spouse/partner/marriage wording until the bond is revealed |
| Formulaic alternatives | “I never imagined,” “I need answers,” etc. | Review context; alternatives can change tense or intent |

Keep established world terms: Alpha King, fated Luna, wolfsbane, house/family names, and project-specific terminology. Do not “naturalize” away rules.

## 3. Optional long-task records

`_localization-progress.md`: project, target, backup, iteration unit, actual episode/scene statuses, current changes, unresolved items, and whole-script consistency check. Do not prepopulate fictional episodes/tasks.

`_localization-log.md`: actual scene, speaker, old/new line, and reason when useful. Do not add empty rows for nonexistent changes. Short excerpts need no separate records.

## 4. Apply versus preserve-and-ask

Apply authorized wording improvements/corrections while preserving meaning, intensity, and voice. Ask only when a new story decision, lock override, or unresolved source choice is necessary. Continue independent work. Do not repeat approvals or force changes to every line/fixed proportion.
