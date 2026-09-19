# Instructions for Claude working in this vault

Read this file, then `START-HERE.md`, before doing anything else in every session.

## What this vault is

A personal "second brain" for security research and bug bounty work — one place that holds everything so nothing has to be re-explained from scratch each session.

## Rules

- **Always read `START-HERE.md` first.** It has the current state of things.
- **Always update `START-HERE.md` before ending a session** — what got done, what's in progress, what the next step is. If you don't write it down, it's gone next session.
- **One folder per target/topic.** Don't dump everything into one giant file — use the templates in `templates/` as the shape for each new target folder.
- **Be honest about "ruled out."** A clean/negative result is just as valuable to record as a confirmed finding — it stops you (or the AI) from re-investigating the same dead end later. Use `templates/ruled-out.md`.
- **Keep a running journal.** Use `templates/journal.md` per target — short, dated entries, not a polished report. The polished report comes later, once something's actually confirmed.
- **Never submit/send/publish anything without being explicitly told to.** This vault is for research and drafting. A human decides what actually goes out the door.

## How to start a new target

1. Copy the four files from `templates/` into a new folder named after the target.
2. Fill in `target-profile.md` with what you know so far.
3. Use the `hypothesis-and-dedup-check.md` prompt (in the `prompts/` folder of the starter kit) before spending real time on any lead.
4. Log everything — including dead ends — in `journal.md` and `ruled-out.md` as you go.
5. Update `START-HERE.md` at the vault root so the next session knows where things stand.
