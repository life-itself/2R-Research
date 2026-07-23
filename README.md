# 2R Research

Evidence-backed Logical Thinking Process model for the Second Renaissance
Research Circle.

The repository distinguishes three related systems:

1. **2R proper** seeks durable cultural transformation.
2. **The 2R Research Circle** improves the shared model that guides inquiry and
   action.
3. **A future federation of individual and group trees** may support emergent
   alignment without imposing one group's tree as the universal tree.

For the Research Circle, the provisional throughput unit is:

> A reviewed, provenance-preserving improvement adopted into the shared 2R LTP
> model because of a research contribution.

This is not a count of meetings, papers, presentations, proposed changes, or
AI matches. A rejected or disputed proposal can still be valuable learning,
but only adopted model improvements count as throughput.

## Repository contents

- `docs/prompts/LTP_BACKGROUND_PROMPT.md` — authoritative project motivation
  and research-group boundary.
- `docs/ltp_trees/` — the pre-existing organization-level Second Renaissance
  trees, retained as prior work and reference material.
- `ltp/` — a fresh Project LTP analysis centered specifically on the Research
  Circle and the contribution-to-model uptake loop.

`ltp/ltp-model.yaml` is the canonical shared causal model. The Markdown files
are readable views of that same model.

## Local dashboard

From the `logical-thought-process-issue-trees-app` repository, run:

```bash
python3 skills/project-ltp/scripts/serve_dashboard.py \
  --project /Users/davidjoseph/github/2R-Research \
  --open
```

The dashboard is local and read-only. When the preferred port is occupied, the
server automatically selects the next available port.

