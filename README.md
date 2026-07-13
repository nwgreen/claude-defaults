# claude-defaults

My global working-style rules for Claude Code, version-controlled and applied to
every project via a symlink.

[`CLAUDE.md`](CLAUDE.md) is the canonical file. Claude Code loads
`~/.claude/CLAUDE.md` into **every** session, in every project, existing and
future. By symlinking that path to this repo, editing the repo instantly updates
the rules everywhere.

## New-machine setup

```
cd ~/Code
git clone git@github.com:nwgreen/claude-defaults.git
ln -s ~/Code/claude-defaults/CLAUDE.md ~/.claude/CLAUDE.md
```

That's it — the next Claude Code session on that machine picks up the rules.

Notes:
- The symlink is **per machine** (it points at a local path), so re-run the `ln`
  on each new machine. The repo travels; the symlink doesn't.
- If `~/.claude/CLAUDE.md` already exists, move it aside first — `ln -s` won't
  overwrite an existing file.
- A session already running won't see edits until it restarts.
- Per-project `CLAUDE.md` files still load **in addition** and can override these
  defaults.

## Editing the rules

Edit [`CLAUDE.md`](CLAUDE.md) here, then commit and push to keep GitHub in sync.
Because `~/.claude/CLAUDE.md` is a symlink, the change is live locally the moment
you save.

## Conventions these rules establish

Beyond brevity/formatting, the working style asks each active project to keep two
running files in its root:

- **`theStory.md`** — an append-only, colorful narrative of how the project came
  to be (want → routes considered → direction & why). Updated after real build
  chunks.
- **`theLooseEnds.md`** — the live "open loops" ledger: things asked for but not
  landed (blocked, awaiting an answer, dropped, or deferred), with enough context
  to resume later. See this repo's own [`theLooseEnds.md`](theLooseEnds.md).
