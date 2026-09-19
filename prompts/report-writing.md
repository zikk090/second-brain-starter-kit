# Prompt: turn a confirmed finding into a clean report

Use this once you've actually verified something works — not before.

---

I've confirmed the following finding on [target name]: [describe what you found and how you verified it].

Please write it up as a clear report with these sections:

1. **Summary** — one or two sentences, plain language, what the bug is and why it matters.
2. **Root cause** — the specific technical reason it happens, with exact file/line/endpoint references where possible.
3. **Steps to reproduce** — numbered, dead-simple, something a stranger could follow with no extra context.
4. **Impact** — what a real attacker could actually do with this, stated honestly (don't oversell it, don't undersell it).
5. **Suggested fix** — a concrete direction, not just "add validation."

Do not draft any actual submission to the vendor/platform yet, and do not claim anything I haven't actually verified — flag clearly if any part of this is inferred rather than tested. Save the result into this target's folder and update `START-HERE.md` to note it's ready for review.
