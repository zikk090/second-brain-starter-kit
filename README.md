# Build Your Second Brain

![Animated node graph](./assets/graph-animation.svg)

**For the human:** this repo builds a memory system *for your AI* — not a journal for you to read. Give it to your AI assistant (Claude, Codex, or anything similar) with the prompt below, answer a few questions honestly, and it builds and maintains its own working memory of your projects from then on, updating itself every time it works. You don't have to maintain it. You don't even have to read it, though you can.

> **The one prompt:** "Go to this repo, read the readme and begin the process of creating a second brain for yourself to help me manage my workload."

## Requirements

An AI assistant that can read and write files, pointed at this repo. That's it. The AI figures out the rest as it goes — that's the whole point of what follows.

---

## Instructions for the AI

*(This section is written to you, the AI reading this. Follow it directly.)*

This is not a document for the human to read and organize by hand — it's a memory system **for you**. You are the one who reads it at the start of every session, writes to it as you work, and refers back to it instead of asking the person to re-explain themselves. Build it, use it, and keep it current, all on your own initiative.

Before creating anything, ask the person a few questions so this gets built for *them*, not left generic:

1. What kind of work do you want this to help manage? (security research/bug bounty, writing, running a business, academic research, general life admin — anything.)
2. Where should the vault folder be created, and do you already use Obsidian, Notion, or neither?
3. What are the 3-5 recurring "things" you track in this work? (Their own words — a novelist tracks manuscripts and submissions, a consultant tracks clients and engagements, a security researcher tracks targets and findings.)

**Then generate fresh files tailored to what they told you. Do not copy the example folder's content and just rename a few words.**

`example-security-research/` in this repo is a single **worked illustration**, for a security-research/bug-bounty workflow specifically — it exists so you can see the *shape* of a good setup, not so you can reuse its wording for someone doing something completely different. The shape is:

- a **status file** (`START-HERE.md`) that always summarizes current state in a few lines, gets *overwritten* (not appended to) every session, and is the first thing you read when you pick work back up
- an **instructions file** (named per your own tool's convention — see "More than one AI" below) telling you how to behave in this specific vault
- a **`templates/` folder** with one fill-in-the-blank template per recurring unit of work they described in question 3 — named and shaped around *their* vocabulary, not the example's
- optionally, a **`prompts/` folder** with ready-made prompts for whatever recurring actions their workflow involves (the example's versions — kicking off research on a new target, sanity-checking a lead, writing up a finding — show what these look like for security research; invent equivalents for their domain)

Build all of this in the location they gave you, using their own words throughout — the security-research example should be unrecognizable in the final result unless that's literally what they're doing.

Once it's built, explain back to them briefly what you made and how you'll use it going forward.

## More than one AI

If the person uses more than one AI assistant against the same vault (say, one for chat-based work and one for terminal/coding work), don't build two separate memories — build one, and give each tool its own entry point into it using whatever filename convention that tool expects (for example, some tools look for `CLAUDE.md`, others for `AGENTS.md`). Keep the content identical or near-identical across those files, and have all of them point back to the same `START-HERE.md` and the same `templates/`/`prompts/` folders. One memory, multiple doors into it.

## Using this on more than one device

This is a plain folder of text files, so `git` is the easiest way to keep it in sync across machines:

```bash
cd /path/to/the/vault
git init
git add .
git commit -m "initial vault"
```

Then create a **private** remote (GitHub, GitLab, wherever) and push to it — private, not public, because from this point on the folder holds real, personal, or work-specific content that's meant for the AI reading it, not for public viewing:

```bash
git remote add origin <your-private-repo-url>
git push -u origin main
```

On another device, `git clone` that same private repo and point the AI at it there. Commit and push at the end of a session, pull at the start of the next one, same as any other git workflow.

## Connecting to Notion

Obsidian (optional) shows *the AI's own* graph of interlinked notes — useful if you want to see the shape of what it's built. Notion is a different kind of optional add-on: a human-friendly dashboard *for you*, separate from the AI's raw working files.

If your AI assistant has a Notion connection available (several AI tools support this natively, or via an MCP/plugin integration), you can ask it to mirror key summaries there — for example, a running table of active projects, or a status page it updates alongside `START-HERE.md`. The vault stays the source of truth the AI reads and writes; Notion becomes the view built for a human to check in on it without opening the raw files.

## What these tools actually are

Quick reference if any of the above is unfamiliar:

- **Git** — a free tool for tracking changes to a folder of files over time and syncing that folder across different computers. It's what almost all software developers use instead of emailing files back and forth.
- **Obsidian** — a free, local note-taking app that turns a folder of plain text files into linked notes with a visual graph view. Nothing is stored on Obsidian's servers; it just displays files that already live on your computer.
- **Notion** — a workspace app for notes, databases, and dashboards, hosted online. A lot of people already use it for personal or team organization, which is what makes it a good "human view" layer on top of the AI's own vault.
