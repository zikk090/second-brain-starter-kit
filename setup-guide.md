# Setup guide — replay the live demo

Five steps, same order as the webinar demo.

## 1. Create a fresh user account (optional but recommended)

This mirrors the demo and gives you a clean environment with no leftover files or settings to confuse the AI.

`System Settings → Users & Groups → Add Account`. Log into the new account.

## 2. Install Claude

- **Easiest**: download Claude Desktop from [claude.ai/download](https://claude.ai/download) and sign in.
- **For the full research workflow** (the one used in this demo): install [Claude Code](https://claude.com/claude-code) instead — it can read/write files directly, run commands, and is what makes the "second brain" pattern actually work hands-off. Requires a terminal; the install command is on that page.

## 3. Create your vault

Pick any folder — Documents, Desktop, wherever. If you want the note-linking/graph-view benefits, open that folder as a vault in [Obsidian](https://obsidian.md) (free). Obsidian is a nice-to-have, not a requirement — the AI just needs a folder of plain Markdown files it can read and write.

## 4. Drop in the starter files

Copy everything from this kit's `vault-starter/` folder into your new vault:

```
your-vault/
├── START-HERE.md
├── CLAUDE.md
└── templates/
    ├── target-profile.md
    ├── hypotheses.md
    ├── ruled-out.md
    └── journal.md
```

## 5. Point Claude at it and go

Open a Claude Code session (or a Claude Desktop project) rooted in that vault folder, and say something like:

> "Read START-HERE.md and CLAUDE.md, then help me start researching [target/topic]."

From here, use the prompts in `prompts/` to drive the actual work. The AI will read `START-HERE.md` at the start of every session and keep it updated as you go — that's the whole trick. You never have to re-explain where you left off.
