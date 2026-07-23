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

## Relationship to Project LTP

This repository is an analyzed project, not a copy of the `project-ltp` skill
itself. Project LTP is a Logical Thinking Process skill that examines a
project's source material, reconstructs its causal logic, and renders several
views of one shared model:

- Goal Tree
- Current Reality Tree
- Evaporating Clouds
- Future Reality Tree
- Prerequisite Tree
- Transition Tree

The portable contract between an analyzed project and the skill's dashboard is
`ltp/ltp-model.yaml`. The Markdown files under `ltp/` are readable views and
supporting analysis derived from that model.

## How this repository was created

This repository was created by:

1. Starting a new repository for the 2R Research Circle.
2. Copying `LTP_BACKGROUND_PROMPT.md` and the existing 2R LTP trees into
   `docs/` as source evidence and prior work.
3. Invoking Project LTP in forward-analysis mode over those materials.
4. Distinguishing 2R proper, the Research Circle, and a possible wider
   federation of trees.
5. Building one evidence-backed causal model with stable entity and link IDs.
6. Generating and validating all six tree views plus the constraint diagnosis,
   assumptions, open questions, and recommended next action.

The generated analysis is a reasoned interpretation of the cited source
material. Its `observed`, `inferred`, `provisional`, `confirmed`, and `disputed`
statuses are intentional and should be preserved when the model is revised.

## Repository contents

- `docs/prompts/LTP_BACKGROUND_PROMPT.md` — authoritative project motivation
  and research-group boundary.
- `docs/ltp_trees/` — the pre-existing organization-level Second Renaissance
  trees, retained as prior work and reference material.
- `ltp/` — the Project LTP analysis centered specifically on the Research
  Circle and the contribution-to-model uptake loop.

`ltp/ltp-model.yaml` is the canonical shared causal model. The Markdown files
are readable views of that same model.

## Visualize this project

The dashboard is supplied by the Project LTP skill, so run its
`serve_dashboard.py` script from wherever the skill is installed. From the
root of this repository:

```bash
python3 /path/to/project-ltp/scripts/serve_dashboard.py \
  --project "$(pwd)" \
  --open
```

For example, if Project LTP is available in another repository at
`skills/project-ltp`, run:

```bash
python3 /path/to/that-repository/skills/project-ltp/scripts/serve_dashboard.py \
  --project "$(pwd)" \
  --open
```

No user-specific filesystem path is required. `--project` identifies the
project to visualize; the script path identifies the Project LTP installation
that supplies the dashboard.

The dashboard is local and read-only. When its preferred port is occupied, the
server automatically selects another available port.

## Visualize any Project LTP analysis

The same dashboard can visualize any project over which Project LTP has been
run, provided that project contains a valid `ltp/ltp-model.yaml`:

```bash
python3 /path/to/project-ltp/scripts/serve_dashboard.py \
  --project /path/to/analyzed-project \
  --open
```

The analyzed project and the Project LTP installation do not need to be in the
same repository. If present, defensible observations in `throughput.yaml` are
also displayed; the dashboard does not require or invent throughput history.
