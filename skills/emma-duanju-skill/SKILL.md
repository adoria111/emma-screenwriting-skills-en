---
name: emma-duanju-skill
description: "Public entry point for Emma Screenwriting Skills. Route requests to installed analysis, adaptation, outlining, refinement, and localization modules and execute the task. Supports 26 professional entries; enable guided mode with at most three questions per round only when requested."
---

# Emma Screenwriting · Main Router

## Guided decision mode (only when requested)

Enable this mode when the user says “walk me through this,” “help me think,” “ask me first,” or explicitly requests questions before drafting. Otherwise, carry out ordinary writing, analysis, and revision requests directly. This mode overrides default continuous execution or fixed questionnaires. Pass it through the main router, compatibility entries, and downstream modules without restarting intake.

1. Read the current material and valid context first. Separate established decisions, locked elements, and genuinely unresolved choices. Do not ask questions already answered. Request only essential missing material; do not invent backstory.
2. Identify the unresolved decisions that most affect the result. Ask at most three independent key questions per round, ordered by impact. Do not hide several questions inside one, pad the count, or steer a multiple-choice question toward a predetermined answer.
3. Explain why each decision matters. When useful, offer two or three directions and explain concretely how they affect characters, relationships, plot, audience anticipation, or the requested deliverable. Allow the user's own direction. An analysis-only request does not require changing the story.
4. Wait for the answers before turning the choices into the authorized proposal. Brief examples may clarify options, but do not deliver the complete solution or decide core creative choices in advance. With partial answers, continue only work independent of the unanswered choices. Silence is not a choice.
5. Briefly restate confirmed decisions, apply them to characters, events, pacing, or the relevant output, and check downstream effects. Ask another round only if important decisions remain. If none remain, explain the existing basis and finish the step without inventing questions.
6. If the user delegates judgment (“you decide”), proceed within that scope while preserving locked elements. Apply the choices to this project, not as automatic rules for other projects.

Starter: “Use [skill name] to walk me through this step. Read my material first and identify the creative decisions that will most affect the result but that I haven't made yet. Ask at most three key questions per round and explain how the options would affect the characters and plot. Don't repeat questions I've already answered. Wait for my answers before developing the proposal.”

Choose and execute the smallest professional method needed for the user's goal. Do not require memorized skill names or routing approval. This router supports 24 regular entries plus two advanced modules; it does not contain or automatically install them. Honor an explicitly chosen module first.

## Locate and read

- Natural-language “Emma screenwriting, help me...” can invoke this entry. Hosts supporting explicit skill syntax may use `$emma-duanju-skill`; this does not imply a matching slash command exists.
- Locate modules through the actual host's skill list/directories or supplied complete files. Read SKILL.md and needed references. Do not assume Claude and Codex share paths or every module sits beside this router.
- Report only methods actually read and used. Name missing modules precisely and continue independent work. Ordinary-method fallback requires agreement and must be distinguished from skill execution.
- “Show capabilities” calls for an explanation; “analysis only” does not edit; “write a prompt first” returns only the prompt; “continue” resumes valid project state. Other action requests should be completed without writing a prompt and asking the user to resend it.

## Route by goal

| Goal | Module | Boundary |
|---|---|---|
| Structure, pace, emotional/information progression | `em-structure` | Read source evidence; no default rewrite. |
| Phase prerequisites, emotional shifts, cross-phase causality | `em-logic-chain` | Read complete scenes; default interactive HTML, analysis only. |
| World rules, occupations, bodies, props, visual effects | `em-worldbuilding` | Separate fact/inference; retain purely visual elements. |
| Reference mechanisms or authorized character/world/event changes | `em-adaptation` | Verify new conditions and downstream effects. |
| Multiple concepts from a brief/premise | `em-iteration` | Do not restart concept selection for a local edit. |
| Series/phase anticipation and payoff chains | `em-expectation` | No need to also run episode hooks automatically. |
| Episode ending, cliffhanger, next opening | `em-episode-hooks` | Check the actual cut and response. |
| Draft episodes from an approved outline | `em-outline-to-script` | Default expansion; preserve core events. |
| Chinese dialogue, character appeal, intent, efficiency | `em-dialogue` | Scene/character assessment, then line scoring/editing. |
| Cut passages, transitions, redundancy | `em-script-trim` | Protect causality, information, necessary emotion. |
| Integrated draft/client-note refinement | `drama-script-refiner` | Protect unapproved content. |
| Legacy dialogue-efficiency request | `em-dialogue-efficiency` | Routes to the same em-dialogue process; do not duplicate. |
| AI-like/literary Chinese working-draft prose | `drama-humanizer` | Expression only; external humanizer-zh dependency. |
| First Chinese-to-US adaptation | `em-us-localization` | Distinct from polishing existing English. |
| Chinese dialogue only into North American English | `drama-dialogue-localizer` | Preserve action and Chinese source. |
| Existing English dialogue polish | `em-english-polish` | Default English-polish entry. |
| Explicit localization-loop request | `drama-localization-loop` | Choose this or English polish as primary; do not double-run. |
| Chinese editorial comments into English Word | `em-comment-transfer` | Transfer comments, do not apply their edits. |
| International concepts and genre combinations | `em-overseas-genre` | Verify time-sensitive market claims separately. |
| Characters, rules, knowledge gaps, sustained conflict | `em-overseas-engine` | Targeted development module. |
| Episode planning and pacing | `em-overseas-beats` | Inherit count, duration, and constraints. |
| Supplied international genre/development references | `em-overseas-reference` | Historical guidance is not current platform policy. |
| Review against applicable guidelines | `em-overseas-review` | No default rewrite or acceptance guarantee. |
| Pitch/submission preparation | `em-overseas-pitch` | No automatic external sending. |
| Core outline, character dossiers, episode outlines | `em-story-architect` | Advanced module; verify it is installed. |
| Advanced scene writing and production-mode rules | `em-chief-writer` | Use when selected/needed; do not duplicate default expansion. |

Connect compound tasks by dependency and pass confirmed facts/constraints between stages. A reference-to-new-script task may use structural analysis, adaptation, and outline expansion. A beats-only task stops before script drafting. A local dialogue request does not load every skill.

## Public-edition compatibility

- Choose `em-logic-chain` versus structure analysis according to the goal. A hook-only task does not require whole-series causal analysis. Shared verified facts do not replace the selected module's coverage requirements.
- “Emma worldbuilding” means `em-worldbuilding`; another package's `drama-worldbuilding-extractor` does not prove this module is installed.
- Since 2026-11-11, `em-dialogue-efficiency` is a compatibility entry for `em-dialogue`. Install both. The 26 professional directories include this alias, not two independent dialogue workflows.
- Refinement is named `drama-script-refiner`. Map legacy `em-script-refine` references to that installed module within this package.
- `drama-truesource` is not bundled. If absent, directly check the designated source, version agreements, protected elements, and approved scope. Read an existing pointer; proceed with a clear sole source. Ask only about substantive unresolved version conflicts.
- Advanced modules live under `advanced/story-writing/skills/`; installing regular entries does not install them.
- `humanizer-zh` is external, not bundled. Disclose its absence for the complete chained humanizer workflow.
- No private material library, fixed local absolute path, hidden module, or automatic skill modification is required.

## Cross-stage collaboration

Distinguish revising existing text, designing new plot, and expanding an approved outline. New continuations need a verified event chain; local sentence-edit methods are insufficient. A reference difference does not authorize rearranging a locked outline.

Separate source facts, transferable functions, and new proposals. Recheck why choices work when changing danger, professional authority, prop function, or character knowledge. Matching episode numbers does not replace causal judgment.

Translate feedback into its intended effect. “Tighter” does not mean removing necessary reasons; “more agency” does not mean never feeling fear; “stronger exchange” does not mean adding two confrontations to every scene. Do not make one note a universal series ban.

For long tasks retain brief state: current draft, confirmed facts/preferences, allowed changes, rejected proposals, dependencies. Save in an authorized workspace or provide a short handoff if files are unavailable. Do not repeatedly turn whole conversations into rules or create a ledger for a simple sentence edit.

Distinguish pasted replacements from excerpts. Preserve deliberate deletions; do not restore from old versions. Ask only when real ambiguity changes the result. Do not assume omissions are accidental or promote every pasted passage to a whole-series final draft.

For narrated drama, follow the current agreement: narration may carry necessary transitions, motives, and anticipation; action/dialogue carry the central exchange and payoff. Do not mechanically restate dialogue. First-person knowledge follows the project's narrative mode without leaking locked secrets. Ordinary scripts do not automatically become narrated drama.

## Completion

Check causality, knowledge, relationships/voices, outline coverage, neighboring responses, and length at the requested scale. Per-episode constraints need individual checks; averages cannot hide missing episodes or major imbalance. Fix routine redundancy directly; cutting key events needs authorization.

Deliver the complete current artifact with only useful located evidence, substantive changes, and unresolved issues. Avoid unnecessary full diagnostic tables. Report reading, execution, and output validation honestly. “Used a skill” is not a quality guarantee, and no tool invocation or test result may be invented.
