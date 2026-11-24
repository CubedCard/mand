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

Copy `skills/mand` into your agent's skills directory, for example:

```sh
# GitHub Copilot CLI (user-level)
copilot skill add ./skills/mand/SKILL.md

# Claude Code (user-level)
mkdir -p ~/.claude/skills && cp -r skills/mand ~/.claude/skills/
```

Then invoke with `/mand` or ask for "mand mode".
