# mand

> "Kan het korter?" — "**Mand!**"

An agent skill that makes your AI coding assistant answer short. Very short. 

## The meme

In 2012, in VPRO's *Omroep Maxim*, presenter Maxim Hartman asks antique dealer Ben Strik to present a small Tichelaar ceramic basket. Then he asks for a shorter version. And shorter. And shorter. Until Strik shouts the entire pitch in one word: **"Mand!"** ("Basket!").

This skill skips straight to the short version.

## Levels

| Level | Example: "Why does my component re-render on every keystroke?" |
|---|---|
| `kort` | The parent passes a new object literal as a prop on every render, so the shallow comparison always fails. Wrap it in `useMemo`. |
| `korter` (default) | New object prop each render. Shallow compare fails. Wrap in `useMemo`. |
| `nog-korter` | Inline object prop. `useMemo` it. |
| `mand` | `useMemo`. |

Say "korter" to go one level down, "kan het langer?" to go one up, "stop mand" to turn it off.

Code, commands, paths, and errors are never shortened. Security warnings, destructive actions, and anything written to files, commits, or PRs stay in full sentences.

## Install

From the root of this repository, install once for Codex, Copilot CLI, Cursor (local), Gemini CLI, OpenCode, and Pi:

```sh
mkdir -p ~/.agents/skills && cp -r skills/mand ~/.agents/skills/
```

For Claude Code, use its user-level skills directory instead:

```sh
mkdir -p ~/.claude/skills && cp -r skills/mand ~/.claude/skills/
```

## Activate

| Tool | How to activate |
|---|---|
| Claude Code | `/mand` |
| Codex | `$mand` |
| Copilot CLI | `/mand` |
| [Cursor](https://cursor.com/docs/skills) | Select `/mand` in Agent chat |
| [Gemini CLI](https://geminicli.com/docs/cli/skills/) | Ask for "mand mode" |
| [OpenCode](https://opencode.ai/docs/skills/) | Mention `@mand` in your prompt |
| [Pi](https://docs.pi.dev/latest/skills) | `/skill:mand` |

You can also ask for "mand mode" in plain language. In Cursor, `/mand` attaches the skill to one message; use a Custom Mode to keep it active for the session.
