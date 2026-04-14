---
description: Install The-User-Voice-Types snippets and slash commands into ~/.claude/
---

Install the snippets and slash commands from this repo into the user's home-level Claude configuration. Do all of this without asking for confirmation between steps — just report what you did at the end.

## Steps

1. **Copy slash commands** from `commands/` in this repo into `~/.claude/commands/`:
   - `commands/transcription-errors.md` → `~/.claude/commands/transcription-errors.md`
   - `commands/hands-tied.md` → `~/.claude/commands/hands-tied.md`

   Create `~/.claude/commands/` if it doesn't exist. If either file already exists at the destination, overwrite it (the source is the canonical version).

2. **Append the two snippets** to `~/.claude/CLAUDE.md`:
   - Read `voice-typing.md` and `one-handed-typing.md` from this repo.
   - For each snippet, extract only the content **below** the `---` horizontal-rule separator (skip the repo-README preamble above it).
   - Append both snippets to the end of `~/.claude/CLAUDE.md`, separated by blank lines.
   - Before appending, check whether either snippet is already present (search for a distinguishing phrase like `"Input method: voice typing"` or `"Input method: one-handed or distracted typing"`). If a snippet is already present, skip it and note that in the final report.
   - If `~/.claude/CLAUDE.md` does not exist, create it with just the snippets.

3. **Report** a short summary: which slash commands were installed, whether each snippet was appended or already present, and the final paths touched. Do not print the full contents of the files.

## Notes

- Use the `Read`, `Write`, and `Edit` tools — not shell `cp`/`cat` — so the operations are visible and auditable.
- Do not modify anything else in `~/.claude/CLAUDE.md`; only append.
- If the user is running this from a clone that isn't at `~/repos/github/my-repos/The-User-Voice-Types`, use the current working directory as the source root.
