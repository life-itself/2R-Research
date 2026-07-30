# 2R Research

Evidence-backed Logical Thinking Process model for the Second Renaissance
Research Circle.

The repository distinguishes three related systems:

1. **2R proper** seeks durable cultural transformation.
2. **The 2R Research Circle** — for the time being, David Joseph and Rufus
   Pollock — is trying to get LTP adopted and used, starting with by itself.
3. **A future federation of individual and group trees** may support emergent
   alignment without imposing one group's tree as the universal tree.

The `ltp/` analysis models system 2. Its goal is:

> The 2R movement adopts LTP and benefits from it.

Adoption has two tests, both taken from the 2026-07-24 whiteboard: a non-trivial
subset of the movement is actively using LTP, and LTP is used in shared spaces
such as the forum so that even people who are not "bought in" benefit from it.

The throughput unit is contested, and the analysis records that rather than
resolving it:

- The 2026-07-24 whiteboard says **new users of LTP and its outputs, including
  people who discover 2R through them**.
- The July 2026 exchange between David and Rufus says **duly improved 2R LTP
  trees**.

Neither is a count of meetings, papers, or presentations. Only the second
currently has observable history; the dashboard's generated throughput track for
this project measures it from Git.

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

Three of the six views exist here. The notes' conflict-resolution section is an
empty stub, so no Evaporating Cloud, Future Reality Tree, or Prerequisite Tree is
supported by the current evidence, and none is published.

The portable contract between an analyzed project and the skill's dashboard is
`ltp/ltp-model.yaml`. The Markdown files under `ltp/` are readable views and
supporting analysis derived from that model.

## How this analysis was built

The first version of this analysis (July 2026) worked from
`LTP_BACKGROUND_PROMPT.md` alone. It took the Research Circle's inquiry process
as the system, set the goal as cumulative and action-guiding inquiry, and named
missing revision governance as the constraint.

It was **rebuilt from scratch**, not amended, once David supplied his and Rufus's
own trees — a hand-drawn problem tree and a goal-and-throughput whiteboard. Those
describe a different system with a different constraint, and the earlier reading
did not survive contact with them. The rebuild:

1. Committed both sources under `docs/notes/`, plus a line-numbered transcription
   of the whiteboard, so evidence citations resolve.
2. Set the system boundary to David and Rufus, and the goal to movement-wide LTP
   adoption.
3. Transcribed the problem tree into the Current Reality Tree, correcting two
   causes the notes listed as leaves but which have causes of their own.
4. Named `IC-4`, *no way of committing to action*, as the constraint: it is the
   cause of the only three-flame effect in the notes, and it sits inside a
   reinforcing loop rather than downstream of one.
5. Turned the hypotheses already written in the notes into five transitions.
6. Recorded the contested throughput unit as a contradiction instead of picking
   one silently, and deleted the three tree views no longer supported.

The generated analysis is a reasoned interpretation of the cited source material.
Its `observed`, `inferred`, `provisional`, `confirmed`, and `disputed` statuses
are intentional and should be preserved when the model is revised.

## Repository contents

- `docs/notes/` — David and Rufus's own problem tree and goal/throughput
  whiteboard, the primary sources for the current analysis.
- `docs/prompts/LTP_BACKGROUND_PROMPT.md` — background narrative and the quoted
  forum and throughput exchanges.
- `docs/ltp_trees/` — the pre-existing organization-level Second Renaissance
  trees, retained as prior work and reference material.
- `ltp/` — the Project LTP analysis of David and Rufus as a system: goal tree,
  current reality tree, transition tree, and the supporting diagnosis.

`ltp/ltp-model.yaml` is the canonical shared causal model. The Markdown files are
readable views of that same model.

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
