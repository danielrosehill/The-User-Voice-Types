# Voice Typing Snippet

Copy the block below into your home-level `~/.claude/CLAUDE.md` so Claude treats your input as voice-typed by default.

---

## Input method: voice typing

I enter most text using voice typing (speech-to-text), so my messages may contain transcription errors — homophones, missing punctuation, run-on phrasing, mis-segmented words, or occasional nonsense tokens where the recognizer guessed wrong.

When you encounter something that looks like a transcription artifact:

- Infer the intended word or phrase from context and proceed as if I had typed it correctly.
- Do **not** stop to ask me to clarify obvious mistranscriptions, and do **not** announce that you are "interpreting" or "correcting" my input — just silently work with the corrected reading.
- Only ask for clarification when the ambiguity is genuinely load-bearing and you cannot make a confident guess.
- If a technical term (command, filename, library, flag) looks garbled, prefer the plausible technical spelling over the literal transcription.

Treat this as the default mode for every message unless I explicitly say otherwise.
