# Build Your Second Brain in Claude — Starter Kit

Companion kit for the webinar "Build Your Second Brain in Claude — with a Security Research & Bug Bounty Focus" (Sept 19, 2026).

This is everything you need to replicate the live demo on your own machine, plus the prompts and templates shown (and some bonus ones) so you don't have to type any of it from scratch.

## What's in here

- **`slide-generation-prompt.md`** — the exact prompt used to generate the webinar slides. Reuse it for your own talks.
- **`setup-guide.md`** — the steps from the live demo: new user account → install Claude → set up your vault → connect it. Follow along or replay it later.
- **`vault-starter/`** — drop this whole folder in as the start of your own "second brain." Contains:
  - `START-HERE.md` — the one file every session should read first (this pattern is the whole trick)
  - `CLAUDE.md` — the instructions file that tells Claude how to behave in your vault
  - `templates/` — fill-in-the-blank templates for the research workflow shown in the demo (target profile, hypotheses, ruled-out log, running journal)
- **`prompts/`** — copy-paste-ready prompts for the workflow:
  - `bootstrap-second-brain.md` — hand this to Claude in an empty folder and it builds your vault structure for you
  - `recon-kickoff.md` — starts a structured research session on a new target
  - `hypothesis-and-dedup-check.md` — sanity-checks a lead before you spend real time on it
  - `report-writing.md` — turns a confirmed finding into a clean, submittable write-up

## The core idea, in one sentence

Give the AI **one file it always reads first** (`START-HERE.md`) and **one file that tells it how to behave** (`CLAUDE.md`), and let it read/write the rest of the vault as your research grows — that's the entire pattern. Everything else in this kit is just that idea applied to security research specifically.

## How to actually use this

1. Read `setup-guide.md` and do the five steps.
2. Copy `vault-starter/` into your own Obsidian vault (or just a plain folder — Obsidian is optional, the pattern works with any folder Claude can read).
3. Pick a prompt from `prompts/` and run it.
4. Watch `START-HERE.md` update itself as you work — that's the second brain doing its job.
