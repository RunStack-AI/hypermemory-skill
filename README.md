# HyperMemory Skill

Give AI coding agents persistent memory across conversations, projects, and
development environments.

[HyperMemory](https://hypermemory.io) stores the decisions, constraints, fixes,
and context that matter to your work. This repository publishes the canonical
software-development skill that teaches an AI agent when to recall, store,
update, connect, and report that context.

> Current stable release: [v0.6.5](https://github.com/hypermemory-ai/hypermemory-skill/releases/tag/v0.6.5)

## What the skill does

Once installed, the skill directs a compatible coding agent to:

- recall relevant context before starting work;
- store durable technical facts, decisions, preferences, and outcomes;
- update existing knowledge instead of creating duplicates;
- connect memories to the projects and components they describe;
- keep a chronological activity timeline; and
- report token usage with explicit measurement quality and activity attribution.

The protocol is designed for software engineering work in Codex, Claude Code,
Cursor, and other MCP-capable agent environments.

## Prerequisites

- A [HyperMemory account](https://hypermemory.io)
- A configured HyperMemory MCP connection or an authenticated
  [HyperMemory CLI](https://docs.hypermemory.io)
- An AI agent that supports skills, instruction files, or repository-based rules

Never put API keys or other secrets in `SKILL.md` or your project repository.

## Install

### Install from Git

Use the repository URL when your agent supports Git-based skills:

```text
https://github.com/hypermemory-ai/hypermemory-skill.git
```

For Cursor, add the URL from **Settings → Skills → Add Skill**.

### Install `SKILL.md`

If your tool uses a local skills directory, copy
[`SKILL.md`](https://github.com/hypermemory-ai/hypermemory-skill/blob/main/SKILL.md)
into a skill folder without changing its contents. A typical layout is:

```text
hypermemory-software-development/
└── SKILL.md
```

If your tool uses a single rules or instructions file, include the contents of
`SKILL.md` using that tool's normal import mechanism.

## Verify the installation

Start a new agent conversation and confirm that the HyperMemory tools are
available. The agent should recall relevant memory before substantive work and
record durable context as work progresses.

For release `v0.6.5`, the canonical file has this checksum:

```text
SHA-256 e5e8288ce15dac71404afff372bf04fbe3321622940bfaa6eeef625312fee57c
```

Verify a downloaded copy with:

```bash
shasum -a 256 SKILL.md
```

## Update

Pull the latest repository revision or replace your installed `SKILL.md` with
the file from the newest [GitHub release](https://github.com/hypermemory-ai/hypermemory-skill/releases).
Check the release notes before updating because the operating protocol may
change between versions.

## Repository contents

| File | Purpose |
| --- | --- |
| [`SKILL.md`](https://github.com/hypermemory-ai/hypermemory-skill/blob/main/SKILL.md) | Canonical software-development agent protocol |
| [`README.md`](https://github.com/hypermemory-ai/hypermemory-skill/blob/main/README.md) | Installation, verification, and update guide |

## Links

- [HyperMemory](https://hypermemory.io)
- [Documentation](https://docs.hypermemory.io)
- [SDK](https://github.com/hypermemory-ai/hypermemory-sdk)
- [Releases](https://github.com/hypermemory-ai/hypermemory-skill/releases)
