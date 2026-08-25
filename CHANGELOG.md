# Changelog

Notable changes to the apex-gate2-haiku one-page site. This file begins with the
2026-08-24 entry; earlier changes are recorded in the git history.

## 2026-08-24 — ship-log entry + judge-gate haiku (first ARMED night, D-71)

Marks the first armed overnight run on the existing single static page.

- Ship log gains one entry — `2026-08-23 — first armed night: the queue runs real
  work again` — rendered from a new `ul.shiplog-entries` list that reuses the
  existing monospace ship-log typography.
- One new haiku on the judge gate ("The gate reads the night, / weighs each line
  against the proof— / then lifts, or does not."), appended as a `figure` in the
  same style as the two haiku already on the page.
- The rendered "Haiku on this page" count moves 2 to 3, and the "Last updated"
  stamp moves to `2026-08-24 22:08 Central`.

Mechanism: both values remain build-time literals written into the markup, so the
page still shows when it was last updated without client JavaScript and without a
build step. Residual: the count and the stamp are kept in step by hand, guarded
only by the comment sitting beside them, so a later edit that adds a haiku without
touching the count would render a stale number. Residual: the entry date
(2026-08-23, the night the lane was armed) and the stamp date (2026-08-24, the
build) differ deliberately, and the page does not explain that difference to a
reader.
