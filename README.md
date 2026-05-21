# HyperMemory Skill

Persistent memory for AI coding assistants — across every conversation, every project, every IDE.

## What is this?

This repo contains the **skill file** that teaches AI coding assistants (Cursor, Claude Code, Windsurf, Cline, etc.) how to use [HyperMemory](https://hypermemory.io) as their long-term memory layer.

Once installed, your AI assistant will automatically remember architecture decisions, tech stacks, preferences, people, bugs, and everything else that matters — without you ever having to repeat yourself.

## Install

### Cursor

Add this to your Cursor settings under **Skills** → **Add Skill**:

```
https://github.com/RunStack-AI/hypermemory-skill.git
```

### Other IDEs

Point your assistant's skill/rules system at the `SKILL.md` file in this repo. If your IDE supports git-based skills, use the `.git` URL above.

## Prerequisites

- A [HyperMemory](https://hypermemory.io) account
- The `hm` CLI installed and authenticated (`hm login`)

## How it works

The skill instructs your AI assistant to:

1. **Recall** relevant memory at the start of every conversation
2. **Store** new information as you work (decisions, preferences, facts)
3. **Update** existing knowledge instead of creating duplicates
4. **Connect** related concepts with meaningful relationships

All of this happens silently in the background — no prompting required.

## Links

- [HyperMemory](https://hypermemory.io) — Dashboard & account
- [SDK](https://github.com/RunStack-AI/hypermemory-sdk) — TypeScript/JavaScript programmatic access
- [Docs](https://docs.hypermemory.io) — Full documentation
