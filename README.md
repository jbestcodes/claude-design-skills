# Claude design skills

Two skills for Claude Code:

- **impeccable** (design): critiques, audits and improves web interfaces. It covers layout, typography, colour, accessibility, responsiveness and motion. Use it with `/impeccable audit`, `/impeccable critique`, `/impeccable polish` and the other commands listed in `skills/impeccable/SKILL.md`.
- **humanizer** (writing): rewrites text that sounds AI-generated so it reads like a person wrote it, without changing what it says. It runs only when you type `/humanizer`.

## Install

Copy the folders into your Claude folder, then restart Claude Code.

| From this repo | To (Windows) | To (Mac/Linux) |
|---|---|---|
| `skills/impeccable` | `%USERPROFILE%\.claude\skills\impeccable` | `~/.claude/skills/impeccable` |
| `skills/humanizer` | `%USERPROFILE%\.claude\skills\humanizer` | `~/.claude/skills/humanizer` |
| `agents/*.md` | `%USERPROFILE%\.claude\agents\` | `~/.claude/agents/` |

To use them in one project only, copy them into that project's `.claude/skills` and `.claude/agents` folders instead.

Impeccable also starts on its own during design and UI work. To stop that, add this line under the `name:` line at the top of `skills/impeccable/SKILL.md`:

```
disable-model-invocation: true
```

## Examples

- `/impeccable audit` on a page: scores accessibility, performance, responsiveness, theming and code quality out of 20, with a ranked fix list.
- `/impeccable critique`: a usability review against Nielsen's heuristics.
- `/humanizer` with pasted text, or with a file name to rewrite the file in place.

## Credits and licences

- impeccable 4.1.3 by Paul Bakaus, Apache License 2.0 (`skills/impeccable/LICENSE`).
- humanizer 3.1.0 by Siqi Chen (https://github.com/blader/humanizer), MIT License (`skills/humanizer/LICENSE`). Packaged here as a skill that runs only when typed.
