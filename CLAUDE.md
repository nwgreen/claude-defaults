# Working Style

These apply to hands-on dev work. For quick one-off questions, read-only
exploration, or scratch work, skip the git/to-do workflow — just answer.
Brevity and formatting rules still apply everywhere.

## Brevity
- Maximum brevity, especially in instructions directed at me.
- Emphasize scannability over completeness.
- Use large number emoji (1️⃣ 2️⃣ 3️⃣) for sequential steps directed at me.
- Steps read like a manual, not a script. State the action, not the narration.

## End of every work chunk
End each chunk with one of:
- **Remaining steps (you):** numbered list of what I need to do next, or
- **Next steps (Claude):** options for what you could do next.
Keep it short. I switch between projects and need to re-orient fast.

## Paste-ready snippets
If a chunk references something I'll need to paste (an id, command, token, config value, URL, etc.), append it verbatim at the very bottom — after the to-dos. Label it in plain text, then put **only the pastable value** in the code block so copying it grabs nothing extra.
Example:
id:
```
76tghyre56yd
```

## Terminal snippets
- Start every terminal-bound snippet with a `cd` line into the right folder — I multi-task and won't be in the expected directory.
- Shell is zsh: keep any inline comments zsh-safe (use `#`, never `//` or `;;` mid-line). Don't paste comments into runnable command lines if there's any doubt — put explanation outside the block.

## Linking to web destinations
When a step is to do something on a specific webpage (e.g. "Update the IAP instructions"):
- Include the direct deep link to that exact page whenever possible.
- If no direct link is possible (auth-gated, dynamic, SPA state), give the click chain to get there, e.g. App Store Connect → My Apps → [App] → In-App Purchases → [item].

## Git workflow (when actively building in a repo)
Skip this for read-only analysis, debugging questions, or scratch work.
1️⃣ Commit and push to the remote repo.
2️⃣ Consult the build instructions / to-do list in use.
3️⃣ Add any new to-dos surfaced during the work.
4️⃣ Check off completed items.

## theStory.md (the project's running narrative)
After a chunk of real build work, append 1–3 sentences to `theStory.md` in the
project root (create it if missing). Capture: what was wanted, the routes
considered, and the direction taken and why.
- Keep it colorful and human — this is the offloaded narrative, not the changelog.
- Append chronologically; never rewrite past entries.
- Goal: by completion, `theStory.md` reads as a narrative telling of how the
  application came to be.

## theLooseEnds.md (asked-for but not landed)
When I ask for something we don't actually finish — blocked, waiting on a
question I haven't answered, dropped when I got distracted, or deliberately
kicked down the road — record it in `theLooseEnds.md` in the project root
(create if missing) so I can recover the context later.
- One entry per loose end: date, what I wanted, why it stalled (blocked on X /
  awaiting my answer / deferred / dropped), and enough detail to pick it back up.
- When an item is finally resolved, mark it done or remove it — don't leave the
  ledger lying.
- This is the live "open loops" list, distinct from theStory.md (the
  after-the-fact narrative of what *did* happen).
- If I ask "what did we punt on / what's outstanding," this file is the answer.
