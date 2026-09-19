# Build Your Second Brain

If someone sent you here with the prompt *"Go to this repo, read the readme and begin the process of creating a second brain for yourself to help me manage my workload"* — you're in the right place. This file is written for both you and the Claude helping you build it.

**What you're about to get:** a personal knowledge system that lives in a folder of plain text files (works beautifully in [Obsidian](https://obsidian.md), but doesn't require it) — one that Claude reads at the start of every session and updates as it works, so you never have to re-explain where you left off.

## Instructions for Claude

Before creating anything, ask the person a few questions so this gets built for *them*, not left generic:

1. What kind of work do you want this to help manage? (security research/bug bounty, writing, running a business, academic research, general life admin — anything.)
2. Where should the vault folder be created, and do you already use Obsidian, or should it just be a plain folder?
3. What are the 3-5 recurring "things" you track in this work? (Their own words — a novelist tracks manuscripts and submissions, a consultant tracks clients and engagements, a security researcher tracks targets and findings.)

**Then generate fresh files tailored to what they told you. Do not copy the example folder's content and just rename a few words.**

`example-security-research/` in this repo is a single **worked illustration**, for a security-research/bug-bounty workflow specifically — it exists so you can see the *shape* of a good setup, not so you can reuse its wording for someone doing something completely different. The shape is:

- a **status file** (`START-HERE.md`) that always summarizes current state in a few lines, gets *overwritten* (not appended to) every session, and is the first thing read when work picks back up
- an **instructions file** (`CLAUDE.md`) telling you how to behave in this specific vault
- a **`templates/` folder** with one fill-in-the-blank template per recurring unit of work they described in question 3 — named and shaped around *their* vocabulary, not the example's
- optionally, a **`prompts/` folder** with a few ready-made prompts for whatever recurring actions their workflow involves (the example's `prompts/` — kicking off research on a new target, sanity-checking a lead, writing up a finding — shows what these look like for security research; invent equivalents for their domain, e.g. a writer might want "start a new draft," "check for overlap with a past piece," "prep a submission")

Build all of this in the location they gave you, using their own words for file names, fields, and prompt content throughout — the security-research example should be unrecognizable in the final result unless that's literally what they're doing.

Once it's built, explain back to them briefly what you made and how to use it going forward. If they want the note-linking/graph view, point them to obsidian.md (free) — otherwise the plain folder works fine as-is.

## For humans skimming this instead of pasting it into Claude

Everything above, done for you: point Claude at this repo with the prompt at the top of this file, answer its questions honestly, and you'll get a second brain built around your actual work, not someone else's. `example-security-research/` is there if you want to see a concrete worked example first — browse it, but don't just copy it unless you're also doing security research.
