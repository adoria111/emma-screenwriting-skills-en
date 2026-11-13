# Emma Screenwriting Skills — English Edition

**A practical AI-assisted writing toolkit for vertical-drama and short-form screenwriters.** Develop a premise, analyze a reference, map cause and effect, build anticipation, strengthen episode endings, draft from an approved outline, and refine dialogue while protecting the story you have already chosen.

Created by **Emma Wang**. This independent English edition is for writers working in North America, Europe, and other English-speaking contexts. Choose your actual audience, territory, variety of English, genre, and production format; the toolkit does not treat those markets as interchangeable.

**27 entries:** one main router, 24 regular specialist entries, and two advanced writing modules. The count includes `em-dialogue-efficiency`, a compatibility entry for the two-step dialogue workflow.

[Download the English repository ZIP](https://github.com/adoria111/emma-screenwriting-skills-en/archive/refs/heads/main.zip) · [Browse the skills](skills/) · [Advanced writing libraries](advanced/story-writing/README.md) · [MIT License](LICENSE)

## Start with the problem you have

| Your situation | Start here | What you get |
| --- | --- | --- |
| “I know the idea, but not the story yet.” | `em-story-architect` or `em-overseas-engine` | Characters, causality, a story engine, and an outline |
| “Why does this reference work?” | `em-structure` | Evidence-based structural analysis |
| “How does each turning point become possible?” | `em-logic-chain` | Causal prerequisites, emotional turns, and an offline interactive HTML report |
| “What makes this world distinctive?” | `em-worldbuilding` | Sourced rules, occupations, bodies, props, settings, and visual traits |
| “The audience has no reason to continue.” | `em-expectation` or `em-episode-hooks` | A clear promise, meaningful progress, and an ending that the next episode answers |
| “My outline is ready; I need scenes.” | `em-outline-to-script` | Complete scenes faithful to approved episode events and endings |
| “The English dialogue sounds translated.” | `em-english-polish` | Natural, playable English with consistent character voices |
| “I want help deciding before you draft.” | A relevant module in guided mode | Up to three consequential creative questions per round, then a proposal based on your answers |

You do not have to run every module. The [main router](skills/emma-duanju-skill/SKILL.md) selects the smallest relevant workflow from modules the assistant can actually read.

### A first conversation

After making the relevant files available to your assistant:

```text
Use Emma Screenwriting Skills to analyze the attached episodes.
My audience is [audience], the setting is [place], and the script is in [variety of English].
Focus on what the protagonist wants, what changes, and why the ending makes us want the next episode.
Analyze only. Do not rewrite or invent missing events.
Cite the episode and scene for each important finding.
```

For original English dialogue, you can use `em-english-polish` on the English draft itself. Without an earlier source-language draft, it cannot verify translation fidelity. Chinese dialogue modules retain their original language scope; translating their instructions has not turned them into a different workflow.

## Installation

### An assistant with repository and file access

Give it this instruction:

```text
Install Emma Screenwriting Skills — English Edition from:
https://github.com/adoria111/emma-screenwriting-skills-en

Use the 25 complete skill directories under skills/ and the two directories under
advanced/story-writing/skills/ for the full set of 27 entries.
Verify the skill directory supported by this host instead of guessing a path.
Keep each module's SKILL.md, agents/, references/, assets/, and other bundled resources.
Compare and back up existing same-name skills before replacing anything.
Do not modify unrelated skills.

Verify that every installed SKILL.md and its referenced local files can be read.
Then read the main router and one specialist module and perform a small exercise on material I supply.
Report file installation, host discovery/loading, and actual execution separately.
If a refresh or new session is needed, say so; do not call a file copy a verified successful load.
```

To download the files yourself:

```sh
git clone https://github.com/adoria111/emma-screenwriting-skills-en.git
```

Cloning downloads the repository; it does not install or activate skills in an assistant. Hosts differ in how they discover and load skills. The original slugs are retained, so compare before installing alongside an existing Chinese edition.

### A host with single-skill ZIP upload

Download and extract the repository. Package each desired **complete skill directory** according to that host's current upload requirements, then upload and enable it. Keep the references and assets with the skill. The repository ZIP contains many skills and is not a single-skill upload package. Installing only the router does not install the specialist modules.

### Ordinary chat, including a chat without skill installation

Open the desired `SKILL.md`, provide its method text and the relevant referenced files in the conversation, then add your material and task. If the assistant cannot read a GitHub link, paste or upload the actual content. Typing a skill name alone does not load its instructions. A chat's attachments or saved instructions are not automatically a native skill installation.

State four things: **material, task, protected elements, and deliverable**.

### Updating the two Chinese-dialogue entries only

The included installer handles `em-dialogue` and its compatibility entry; it is not a full-library installer:

```sh
python3 scripts/install-dialogue-skills.py --check
python3 scripts/install-dialogue-skills.py
```

It defaults to `$CODEX_HOME/skills`, or `~/.codex/skills` if that variable is unset. Use `--skills-dir /your/verified/skill-directory` for a different destination. It backs up changed files, preserves an existing directory symlink, checks file contents, and leaves unrelated modules and extra files alone. A restricted environment may lack write permission; downloading from GitHub does not change permissions. Successful file verification does not prove host loading.

## Complete catalog

### Analysis and story development

| Entry | Purpose | Typical deliverable |
| --- | --- | --- |
| [emma-duanju-skill](skills/emma-duanju-skill/SKILL.md) | Route a task and preserve project state across stages | The requested work through the relevant installed methods |
| [em-structure](skills/em-structure/SKILL.md) | Examine conflict, structure, pace, and emotional movement | Located structural findings; no automatic rewrite |
| [em-logic-chain](skills/em-logic-chain/SKILL.md) | Work backward from phase endpoints and trace prerequisites | Interactive HTML, episode summaries, expandable scene evidence |
| [em-worldbuilding](skills/em-worldbuilding/SKILL.md) | Extract world rules and visual identity from existing material | Fact/inference tables with source locations and reusable techniques |
| [em-adaptation](skills/em-adaptation/SKILL.md) | Transfer a reference's function or change approved story dimensions | A new proposal and downstream causal checks |
| [em-iteration](skills/em-iteration/SKILL.md) | Develop distinctive options from a brief, premise, or reference | Concepts, relationships, engines, scene ideas, and escalation |
| [em-expectation](skills/em-expectation/SKILL.md) | Connect series goals, phase tasks, and earned payoffs | Audience anticipation and promise/payoff analysis |
| [em-episode-hooks](skills/em-episode-hooks/SKILL.md) | Diagnose, design, or repair specific episode endings | Audience desire, mechanism, filmable cutoff, and next response |
| [em-outline-to-script](skills/em-outline-to-script/SKILL.md) | Expand an approved episode outline | Full scenes preserving core events and endings |
| [em-script-trim](skills/em-script-trim/SKILL.md) | Remove redundant material | A leaner draft with necessary causality and emotion intact |

### Dialogue, refinement, and localization

| Entry | Purpose | Language or scope boundary |
| --- | --- | --- |
| [em-dialogue](skills/em-dialogue/SKILL.md) | Step 1: scene, character appeal, and intent; Step 2: line efficiency and refinement | Chinese dialogue; English instructions and teaching glosses |
| [em-dialogue-efficiency](skills/em-dialogue-efficiency/SKILL.md) | Compatibility route into the same two-step process | Install with `em-dialogue`; not a second independent pass |
| [drama-humanizer](skills/drama-humanizer/SKILL.md) | Reduce formulaic or literary wording while locking story beats | Chinese working drafts; full chained workflow requires external `humanizer-zh` |
| [drama-script-refiner](skills/drama-script-refiner/SKILL.md) | Apply draft or client-note refinement | Edit only the authorized elements |
| [em-english-polish](skills/em-english-polish/SKILL.md) | Refine meaning, natural speech, performance, and voice | Existing English dialogue; preserve action and source text |
| [drama-localization-loop](skills/drama-localization-loop/SKILL.md) | Review localized English across episodes | An alternative English-polish entry; do not duplicate the same pass |
| [drama-dialogue-localizer](skills/drama-dialogue-localizer/SKILL.md) | Localize dialogue only into North American English | Chinese dialogue input; preserve action and Chinese source |
| [em-us-localization](skills/em-us-localization/SKILL.md) | Establish a first US cultural and English version | Chinese-to-US adaptation within approved changes |
| [em-comment-transfer](skills/em-comment-transfer/SKILL.md) | Translate and place editorial comments in corresponding English Word text | Preserve body text and native comment structure; do not execute the comments |

### Market-specific development and submission preparation

“Overseas” is retained in the original identifiers. Set the actual territory and audience for each project.

| Entry | Purpose | Typical deliverable |
| --- | --- | --- |
| [em-overseas-genre](skills/em-overseas-genre/SKILL.md) | Compare genres and emotional selling points | Concept cards with reasons for the tradeoffs |
| [em-overseas-engine](skills/em-overseas-engine/SKILL.md) | Develop a sustained story | Characters, rules, information gaps, conflict, and payoff |
| [em-overseas-beats](skills/em-overseas-beats/SKILL.md) | Build episode progression | Goals, actions, payoffs, hooks, and candidate cutoff analysis |
| [em-overseas-reference](skills/em-overseas-reference/SKILL.md) | Use the collected genre, case, and development methods | Relevant reference guidance with evidence limits |
| [em-overseas-review](skills/em-overseas-review/SKILL.md) | Review against the supplied or verified brief | Located issues; no promise of acceptance |
| [em-overseas-pitch](skills/em-overseas-pitch/SKILL.md) | Prepare an existing project for review | Positioning, synopsis, characters, outline, and sample package |

### Advanced writing modules

| Entry | Purpose | Included library |
| --- | --- | --- |
| [em-story-architect](advanced/story-writing/skills/em-story-architect/SKILL.md) | Build the core outline, character profiles, and episode outline | Six chapters on opening blocks, emotion, pacing, conflict, hooks, and character development |
| [em-chief-writer](advanced/story-writing/skills/em-chief-writer/SKILL.md) | Write specified episodes from an approved outline | Fourteen chapters, including dialogue, format, live action/AI/animation, reveal boundaries, agency, and delivery review |

## Ask first, then develop the choices

Ordinary work requests are executed directly. To enter guided decision mode, say:

```text
Use [skill name] to walk me through this step.
Read my material first and identify the creative decisions that most affect the result but that I have not made yet.
Ask at most three key questions per round and explain how the options affect the characters and plot.
Do not repeat questions I have already answered.
Wait for my answers before developing the proposal.
```

For example: “Use em-adaptation to help me rethink the two leads' relationship. Ask the important questions first; do not write the outline yet.” To delegate the remaining decisions, say so explicitly.

## What is preserved

The methods distinguish analysis, adaptation, outline expansion, and local refinement. They preserve approved facts, motivations, character knowledge, props, clues, deleted material, and endings unless a change is authorized. They separate source facts from interpretation and new proposals. They treat repeated wording differently when performance, strategy, or relationship changes make the repetition meaningful.

The router coordinates methods; it cannot supply missing modules or guarantee model behavior. `drama-truesource` is not bundled: where appropriate, the modules perform direct authoritative-draft checks instead. `humanizer-zh` is an external dependency for the full humanizer chain; its absence must be disclosed. No private project directory is needed for the bundled general methods.

## Edition and validation

English edition date: **2026-11-13**. Based on the source repository's latest `main` at preparation time: [`82057b23bfcd1c375f525d16c8e834631185e2ca`](https://github.com/adoria111/emma-screenwriting-skills/commit/82057b23bfcd1c375f525d16c8e834631185e2ca).

The source includes the November 12 logic-chain and worldbuilding additions, the November 11 two-step dialogue workflow, guided decision mode, and the advanced writing libraries. This edition translates the current instructions, references, interface metadata, teaching examples, and logic-chain template into English. Slugs remain stable. Chinese working-script examples are explained in English; character counts are not silently treated as English word counts.

Historical Chinese ZIPs are not carried into the English working tree. Use this repository's ZIP for current English files. Historical evaluation records are translated and explicitly labeled; their old hashes and pass statuses do not certify the current English files. See [VALIDATION.md](VALIDATION.md) for the checks actually completed for this edition.

The collected references are editorial methods and case summaries, not current market rankings, platform policies, or guaranteed production capabilities. Complete third-party scripts, course recordings, private projects, and missing source images are not bundled. Analysis of a script does not establish viewer behavior or commercial success.

[Original Chinese repository](https://github.com/adoria111/emma-screenwriting-skills) · [Edition notes](EDITION.md)

## License

The files included here are available under the [MIT License](LICENSE): use, modify, and redistribute them while retaining the copyright and permission notice. The license does not extend to unbundled private material, third-party scripts, source images, or an unrelated course or skill package. “Beta” in some module titles describes their historical method edition, not a shared benchmark certification.
