# plain-language

[Español](README.es.md)

A short set of plain-language rules for AI coding agents, in English and Spanish.
The agent applies them to its replies, docs, comments and commit messages.
You can also ask it to review or rewrite a text in plain language.

The rules follow the four principles of ISO 24495-1: relevant, findable, understandable and usable.
They are original wording, not text from the standard.
They take about 600 tokens, so you can load them in every session.

## Install as a skill

Run:

```sh
npx skills add gecm0/plain-language
```

Or copy `skills/plain-language/` into your agent's skills folder:

| Agent | Folder |
|---|---|
| Claude Code | `~/.claude/skills/` |
| Codex | `~/.agents/skills/` |
| Pi | `~/.agents/skills/` or `~/.pi/agent/skills/` |

## Make it always active

A skill loads only when the agent decides it is relevant.
To apply the rules in every reply, also load the file from the agent's global instructions:

| Agent | File | What to add |
|---|---|---|
| Claude Code | `~/.claude/CLAUDE.md` | `@~/.claude/skills/plain-language/SKILL.md` |
| Codex | `~/.codex/AGENTS.md` | the content of `SKILL.md` |
| Pi | `~/.pi/agent/APPEND_SYSTEM.md` | the content of `SKILL.md` |

Codex and Pi do not support imports, so paste the content or use a symlink to `SKILL.md`.

## License

MIT
