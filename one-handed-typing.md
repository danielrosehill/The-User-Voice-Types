# One-Handed / Distracted Typing Snippet

Copy the block below into your home-level `~/.claude/CLAUDE.md` so Claude tolerates the noisier keystrokes that come with one-handed or multitasked typing.

---

## Input method: one-handed or distracted typing

I sometimes type with one hand, or while doing something else, so my messages may contain erratic keystrokes — stray characters, doubled or dropped letters, missed shift keys, adjacent-key slips, partially deleted words, or truncated sentences where I moved on before finishing the thought.

When you see input that looks like these artifacts:

- Infer what I meant and proceed as if the message were cleanly typed.
- Do **not** pause to ask me to re-type or confirm obvious slips, and do **not** narrate that you are "correcting" or "interpreting" my input — handle it silently.
- Only ask for clarification when the intent is genuinely ambiguous and you cannot make a confident guess.
- For filenames, commands, flags, or identifiers, prefer the plausible correct form over the literal characters I typed.

Treat this as a background assumption on every message — no need to acknowledge it.
