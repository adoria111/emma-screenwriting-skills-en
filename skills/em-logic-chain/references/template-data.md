# Filling the Progress Template

Copy `assets/progress-template.html` to the deliverable and replace every token below. CSS/rendering are embedded; preserve layout and primarily replace content. Any supported local text tool can generate the final single file; no fixed runtime/network package is required.

## Page fields

- `__TITLE__`: page title.
- `__EDITION__`: short edition/purpose.
- `__NAV__`: optional switch-link HTML using `.tab`, current link `aria-current="page"`; empty for one report.
- `__THEME__`: main-plot genre label.
- `__HEADING__`: readable show/report title.
- `__SUBTITLE__`: formal title or short subtitle.
- `__INTRO__`: main driver in one/two sentences.
- `__HINT__`: one-line interaction hint; distinguish paywall from analytical phase where needed.
- `__FOOTER__`: brief source and expandable coverage/thread HTML.
- `__DATA__`: data object below. Serialize JSON, replace `</` with `<\/` before embedding in application/json, and do not HTML-escape the entire JSON.
- `__STATIC__`: complete static HTML for every phase, used for printing/show-all.
- `__FALLBACK__`: equivalent complete no-script content, with IDs distinct from static/live versions.

HTML-escape all other plain-text fields. Replace every token before delivery; the unfilled template is not a finished report.

## Data

Top level: `{"cards":[...]}`. Optional `rewardLabel` and `chainLabel` customize diagnostic subheadings. Each card:

```json
{
  "label": "Phase 1",
  "range": "Episodes 1–9",
  "title": "Short phase objective",
  "state": "Previous state → New state",
  "reward": "One sentence describing the actual payoff.",
  "goal": "What the character wants.",
  "viewer": "What viewers await, as a structural interpretation.",
  "chains": [{
    "title": "One necessary condition",
    "nodes": [{"text":"Initial need"},{"text":"Specific action"},{"text":"Condition established"}],
    "why": "One sentence explaining the mechanism."
  }],
  "emotion": "Trigger, emotional change, and driver in one/two sentences.",
  "bridgeLabel": "Why another phase follows",
  "bridge": "How this result or unresolved issue enables the next phase.",
  "deep": "Safe expandable detail HTML built by the generator."
}
```

After filling state/reward, verify the actual entry/exit scenes. The left side cannot use coronation/recognition achieved midway through this phase. The right side/payoff cannot describe a plan or promise as completed. Put later payoffs in bridge or explicitly label later resolution. Check actual event locations, not merely ranges/field presence.

An issue node may include `"issue":"L1"`; the template adds a pale-brown cue/ID. Explain it in deep/details, not color alone.

## Details and evidence

`deep` is inserted as HTML: use only safe generator-built markup and escape source text first. Organize episode summaries, prerequisites, arrow mechanisms, both parties' emotions, conflicts, and scene records with details/summary.

Example live target: `id="live-scene-1-1"`; link: `href="#live-scene-1-1" data-ref="scene-1-1"`. Clicking opens the target and parent details. Cross-phase references need a target in the selected phase's appendix or another reliable navigation implementation; no broken anchors.

Use different static/no-script ID prefixes and rewrite hrefs. Omit live `data-ref` in those copies. Generate every phase from the same data. Static evidence can appear once at the end; do not supply only Phase 1 fallback.

Before delivery, check all tokens replaced, parsable JSON, valid anchors, expandable complete phase/episode coverage, and no remote dependencies. Keep the first view a thin progress bar plus short horizontal chains, with argument below.
