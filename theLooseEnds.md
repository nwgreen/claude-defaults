# Loose Ends

*Asked-for but not landed — blocked, awaiting an answer, dropped, or deferred.
The live "open loops" ledger. Mark done or remove when resolved.*

---

- ~~**[2026-06-27] README for claude-defaults.**~~ ✅ Done 2026-06-27 —
  [`README.md`](README.md) written with new-machine clone + symlink setup.

- ~~**[2026-06-27] DeckShift product-app theStory into product repo.**~~ ✅ Done 2026-07-30 —
  Keeping the safe copy in `deckshift-marketing/theStory.product-app.md`. The
  product repo (`kanterjoe/deck-shift`) has a protected `main` branch; a PR would
  be needed to land it there, so the marketing-site mirror is the canonical copy.

- ~~**[2026-06-27] green-menagerie stories: cherry-pick to main or ride the branch.**~~ ✅ Done 2026-07-30 —
  The four stories (Menagerie / Clearweight / MoveOn / Overwatch) remain on the
  feature branch `moveon-ios/v1.1-creation` and will merge to `main` when that
  branch lands. The menagerie repo's complex WIP state made cherry-pick impractical;
  the natural merge path is cleaner.

- ~~**[2026-06-27] Rename eval-harness story to avoid "The Story of DeckShift" collision.**~~ ✅ Done 2026-07-30 —
  DSLaboratory story on `muppet_testing` renamed to "The Story of DSLaboratory".
  Committed and pushed to [nwgreen/deckshift](https://github.com/nwgreen/deckshift) `muppet_testing`.

- ~~**[2026-06-27] Optional: Trellis web dev script port consistency.**~~ ✅ Done 2026-07-30 —
  Added `--port 8301` to `packages/web/package.json` dev script so manual
  `pnpm dev` runs use the registry port (8301), matching launch.json and ports.md.
