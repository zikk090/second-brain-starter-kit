# Prompt: sanity-check a lead before investing real time

Use this before you sink hours into a hypothesis — it's much cheaper to find out now that something's already known or already dead.

---

Before I spend real time on this hypothesis: [describe the lead/theory in a sentence or two].

Please:

1. Check `ruled-out.md` and `hypotheses.md` for this target — has this exact idea, or something close to it, already been tried or dismissed?
2. Search for prior art: existing CVEs, public disclosed reports, GitHub issues/PRs, or advisories that might already cover this exact behavior.
3. Give me an honest read: is this genuinely novel, a likely duplicate, or already fixed/mitigated? If you're not sure, say so rather than guessing confidently.
4. If it's worth pursuing, suggest the smallest concrete test that would confirm or kill it — I want to fail fast if it's going to fail.
5. Log your conclusion in `hypotheses.md` (or move it straight to `ruled-out.md` if it's already dead) so this check doesn't have to happen twice.
