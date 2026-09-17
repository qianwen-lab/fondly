# Tide Private V8.9

This is an update for the ORIGINAL PRIVATE Tide repository. Do not upload it to Tide-Beta.

- Storage remains `tide.v1`, schema remains 11. Existing goals, days, reviews and End Goal remain intact.
- Forecast: robust 7-calendar-day trend, median-of-pairwise-slopes over recent 14–21 days, decaying pace with a retained trend so the curve does not artificially stop just above the target. A specific reach date is shown only if the fitted trend reaches the goal within 120 days; otherwise the UI says `No date yet` or `> 120 days` with a clear reason. Projections are not guarantees. Original plotted weigh-ins are unchanged.
- Food context: one pink chart dot now represents `Eating out / alcohol / snacks`; the detailed line identifies which one(s). Use the `Snacks` tag in the same Life events row to record snacks, which reuses the existing `food.noSnack` field; the existing `No snacks` daily tracker still works.
- BM removed from Life events and Progress and from goal review export. Old stored BM fields are preserved in the full JSON backup for compatibility and are not silently deleted.
- Period is unchanged as an optional Life event tag; no new period logic has been added without approval.
- Eight flat files. Replace the eight files in the PRIVATE Tide repository only; refresh the installed web app after publishing. Export a backup first.
