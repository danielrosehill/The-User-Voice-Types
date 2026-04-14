# The-User-Voice-Types

[![Claude Code Repos Index](https://img.shields.io/badge/Claude%20Code-Repos%20Index-blue?style=flat-square&logo=github)](https://github.com/danielrosehill/Claude-Code-Repos-Index)

Drop-in snippets and slash commands for Claude Code users who dictate or type messily. They tell Claude to silently infer around transcription errors and erratic keystrokes instead of stopping to ask.

## Why this exists

A lot of real-world prompting happens in situations where input quality is terrible:

- **Voice typing** while walking, driving, or just to go faster — transcription garbles homophones, technical terms, and punctuation.
- **One-handed typing** while parenting, holding a coffee, on a phone, or multitasking — stray keystrokes, dropped words, truncated sentences.

Without context, Claude tends to either take the mangled input literally or stop to ask for clarification. Both are friction. These snippets and commands tell Claude, once, to just infer around the noise and keep moving.

## CLAUDE.md snippets

Paste one or both into `~/.claude/CLAUDE.md` so the instruction applies to every session.

| Snippet | When to use |
|---|---|
| [voice-typing.md](voice-typing.md) | You dictate most messages via speech-to-text. |
| [one-handed-typing.md](one-handed-typing.md) | You sometimes type one-handed or while multitasking. |

## Install

Clone this repo, open Claude Code inside it, and run:

```
/install
```

That installs both slash commands into `~/.claude/commands/` and appends both snippets to `~/.claude/CLAUDE.md`. See [`.claude/commands/install.md`](.claude/commands/install.md) for exactly what it does.

## Slash commands

For moments when you can't edit `CLAUDE.md` and just need to flag the current situation quickly — without fumbling for the keyboard to explain yourself.

Installed by `/install`, or copy the files in [`commands/`](commands/) to `~/.claude/commands/` manually.

| Command | Purpose |
|---|---|
| `/transcription-errors` | "That last message was voice-typed and came out garbled — infer around the errors." |
| `/hands-tied` | "My hands are occupied (parenting, etc.) — expect typos for the next while, just infer around them." |

Both commands tell Claude to handle the situation silently: no "I interpreted that as…" preambles, no clarification requests for obvious slips.

---

For more Claude Code projects, visit [my index](https://github.com/danielrosehill/Claude-Code-Repos-Index).
