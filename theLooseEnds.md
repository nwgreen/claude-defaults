# Loose Ends

*Asked-for but not landed — blocked, awaiting an answer, dropped, or deferred.
The live "open loops" ledger. Mark done or remove when resolved.*

---

- ~~**[2026-06-27] README for claude-defaults.**~~ ✅ Done 2026-06-27 —
  [`README.md`](README.md) written with new-machine clone + symlink setup.

- **[2026-06-27] DeckShift product-app theStory into its own repo — blocked.**
  The product-app story is mirrored into `deckshift-marketing/theStory.product-app.md`
  because `kanterjoe/deck-shift` `main` is protected (direct push rejected,
  `GH013`). To land it in the product repo, push a branch (`add-the-story`) and
  open a PR. The original commit `0959c0a` is dangling and will be GC'd — the
  marketing-repo mirror is the safe copy.

- **[2026-06-27] green-menagerie stories on a feature branch — awaiting your call.**
  The four stories (Menagerie / Clearweight / MoveOn / Overwatch) were committed on
  branch `moveon-ios/v1.1-creation`, not `main`. Decide whether to cherry-pick them
  to `main` now or let them ride with that branch's merge.

- **[2026-06-27] Duplicate "The Story of DeckShift" title — awaiting your answer.**
  The eval-harness `theStory.md` on DeckShift's `muppet_testing` branch is titled
  "The Story of DeckShift," same as the product-app story. Offered to rename it
  (e.g. "The Story of DSLaboratory") to avoid mix-ups; no answer yet.
