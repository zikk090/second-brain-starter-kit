# Build Your Second Brain

If someone sent you here with the prompt *"Go to this repo, read the readme and begin the process of creating a second brain for yourself to help me manage my workload"* — you're in the right place. This file is written for both you and the Claude helping you build it.

**What you're about to get:** a personal knowledge system that lives in a folder of plain text files (works beautifully in [Obsidian](https://obsidian.md), but doesn't require it) — one that Claude reads at the start of every session and updates as it works, so you never have to re-explain where you left off.

## Instructions for Claude

Before creating anything, ask the person a few questions so this gets built for *them*, not left generic:

1. What kind of work do you want this to help manage? (security research/bug bounty, writing, running a business, academic research, general life admin — anything.)
2. Where should the vault folder be created, and do you already use Obsidian, or should it just be a plain folder?
3. What are the 3-5 recurring "things" you track in this work? (For security research: targets, leads, findings. For a writer: projects, drafts, submissions. For general life: areas, projects, tasks.)

Then, in the location they gave you:

1. Create a **`START-HERE.md`** — the one file that always summarizes current state in a few lines, gets *overwritten* (not appended to) every session, and is the first thing to read when work picks back up.
2. Create a **`CLAUDE.md`** with instructions for yourself, tailored to what they told you: always read `START-HERE.md` first, always update it before ending a session, keep one folder per recurring unit of work, log dead ends/rejected ideas as honestly as wins, and never send/submit/publish anything without being explicitly told to.
3. Create a **`templates/`** folder with fill-in-the-blank templates matching their actual workflow. Use this repo's `vault-starter/templates/` as your reference shape — it's a worked security-research example (`target-profile.md`, `hypotheses.md`, `ruled-out.md`, `journal.md`) — but rename and reshape the fields to whatever they actually track.
4. **If they're doing security research or bug bounty work specifically**, also copy the ready-made prompts from this repo's `prompts/` folder into their vault — they're built for exactly that workflow (kicking off recon on a new target, sanity-checking a lead before wasting time on it, and writing up a confirmed finding).
5. Explain back to them, briefly, what you built and how to use it going forward. If they don't already use Obsidian and want the note-linking/graph view, point them to obsidian.md (free) — otherwise the plain folder works fine as-is.

## For humans skimming this instead of pasting it into Claude

Everything above, done for you: point Claude at this repo with the prompt at the top of this file, answer its questions honestly, and you'll have a working second brain in a few minutes. `vault-starter/` and `prompts/` are the reference material Claude builds from — copy them by hand instead if you'd rather skip the conversation.
