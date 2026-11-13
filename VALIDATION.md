# English-edition validation

Date: 2026-11-13. Source baseline: `82057b23bfcd1c375f525d16c8e834631185e2ca`, rechecked against the source repository's `main` before publication.

## Completed checks

| Check | Result |
| --- | --- |
| Entry coverage | All 27 original skill identifiers retained: one router, 24 regular specialist entries, two advanced modules |
| Skill frontmatter | All 27 passed the skill-creator basic validator |
| Interfaces | 27 English `agents/openai.yaml` files; valid YAML; descriptions within 25–64 characters; prompts name the corresponding skill |
| English working tree | Text and filenames scanned for residual CJK characters; none remain |
| Data | All JSON files parse; historical test records explicitly identify their provenance |
| Local resources | Markdown file links resolve; each skill retains its bundled references and assets |
| Long references | Six Story Architect chapters, fourteen Chief Writer chapters, nine genre cards, six case notes, and all fifty C05 episode rows retained |
| Dialogue installer | Temporary-directory dry run, eight-file content verification, repeat-run idempotence, and backup before replacement passed |
| Whitespace | `git diff --check` passed |

## Independent forward exercises

An independent executor read the actual English methods and worked from small fictional requests rather than an expected answer.

- **Worldbuilding:** extracted an occupation, prosthetic materials/light, a maintenance-price complaint, a scanning sequence, and purely visual foreground chains. It distinguished the client's claim from a universal economic rule and did not invent an energy source, diagnosis, or sabotage.
- **Episode hooks:** recognized that an award already shown to viewers shifts anticipation toward public recognition and the promised workshop transfer. It did not call the known result a new mystery or claim an unwritten continuation was verified.
- **Logic chains:** produced an offline HTML report covering three episodes and six scenes in two nonoverlapping phases. It preserved the stated paywall after Episode 2, placed the actual access payoff in Episode 3, identified causal/disclosure gaps, and left the buyer and later outcome unknown.

The first exercise exposed untranslated references and template labels during preparation. Those files were translated before the final scan. The logic-chain report was generated from the final English template.

## HTML checks

The generated test report passed embedded JSON parsing, placeholder replacement, complete scene coverage, evidence-anchor checks, duplicate-ID checks, static/no-script coverage, and a scan for external resource dependencies. JavaScript syntax passed. A lightweight DOM-stub runtime exercise covered rendering, phase bounds, phase/navigation buttons, evidence expansion, full-view/return controls, and print hooks.

Visual browser testing remains unverified: the installed headless browser aborted before rendering, and the available in-app browser could not be opened. The runtime checks do not establish visual appearance, keyboard behavior in a real browser, print layout, or narrow-screen overflow.

## Limits

These checks establish package structure and selected behaviors, not a cross-model benchmark, a complete literary-quality evaluation, or successful installation in every host/account. Historical evaluation files are translated records of earlier Chinese tests; their pass labels and hashes are not new English-edition test results. No commercial, audience-retention, platform-approval, or current market claim was validated.
