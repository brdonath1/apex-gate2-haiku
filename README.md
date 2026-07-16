# apex-gate2-haiku

A single static one-page site that shows today's date and an original haiku
about shipping software. GATE-2 trial deliverable for the Apex unattended
overnight chain (preflight → build → cross-model review → deploy → report).

- **Entry point:** [`index.html`](index.html) — one file, inline CSS, no build
  step, no external network calls. Open it directly (`file://`) or serve the
  directory statically.
- **Date:** rendered client-side from the viewer's clock, so it always shows
  the current day (and self-refreshes if a tab is left open across midnight).
  Nothing is hard-coded; with JavaScript disabled the page invites the viewer
  to enable it rather than assert a stale date.
- **Deploy:** GitHub Pages (see the deployment's live preview URL in the
  morning report).

Built via the MetaSwarm orchestrated pipeline — writer lane `claude`,
cross-model adversarial review by `codex` (gpt-5.6-sol) and `gemini` (pro).
