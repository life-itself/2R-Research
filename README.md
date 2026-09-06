# 2R Research

Evidence-backed Logical Thinking Process model for the Second Renaissance
Research Circle.

**Where the model lives (since 2026-09-06).** The live model is the Reason
Commons space *Reason Commons Focus*, which is connected to this repository:
<https://reason-commons.lovable.app/app/spaces/365f2925-1a97-4367-8df2-e76a7757540e>.
Every sync exports it here as
`.reason-commons/365f2925-1a97-4367-8df2-e76a7757540e.ltp.json` — the full
interchange document with its version series and event history — and projects
the transition tree's actions onto this repository's issues, which the platform
opens, labels and reconciles itself. The `ltp/*.md` files are the July 2026
analysis by the now-retired `project-ltp` skill, kept for the record and no
longer maintained; the `ltp/ltp-model.yaml` they were rendered from, and the
hand-run issue ledger beside it, were removed on 2026-09-06 because the space
had superseded them and the copy no longer matched what the team accepts.

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

Neither is a count of meetings, papers, or presentations. Only the second has
observable history. The reasoncommons.com dashboard used to count it from this
repository's Git history; that track was retired with the dashboard project on
2026-09-06, and the measure now belongs in the space's own ratified throughput
definition, which has not been defined yet.

## Relationship to Project LTP (historical)

The July 2026 analysis under `ltp/` was produced by the `project-ltp` skill,
now deprecated in favour of `ltp-project`, which writes the Reason Commons
interchange format directly. Project LTP examined a project's source material,
reconstructed its causal logic, and rendered several views of one shared model:

- Goal Tree
- Current Reality Tree
- Evaporating Clouds
- Future Reality Tree
- Prerequisite Tree
- Transition Tree

The Markdown files under `ltp/` are readable views and supporting analysis
derived from the model as it stood in July 2026.

Three of the six views exist here. The notes' conflict-resolution section is an
empty stub, so no Evaporating Cloud, Future Reality Tree, or Prerequisite Tree is
supported by the current evidence, and none is published.

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
- `ltp/` — the July 2026 Project LTP analysis of David and Rufus as a system:
  goal tree, current reality tree, transition tree, and the supporting
  diagnosis, kept for the record.
- `.reason-commons/` — the current model, exported by the Reason Commons
  platform from the connected space on every sync. This is the canonical file.

## Read the current model

Open the space at
<https://reason-commons.lovable.app/app/spaces/365f2925-1a97-4367-8df2-e76a7757540e>,
or read the exported `.reason-commons/365f2925-1a97-4367-8df2-e76a7757540e.ltp.json`
in this repository. The export is the interchange document described in the
Reason Commons import specification: current standing with its status and
validity, the role hierarchy, relationships and their assumptions, accepted
conclusions, and under `history` the superseded wordings, the accepted version
series with its digest chain, and the event stream with the actor behind each
change. It can be re-imported into any Reason Commons space, and the same
document is available from the app as a YAML dialect.

The transition tree's actions are this repository's open issues labelled
`rc:ready` (or `rc:blocked`, `rc:awaiting-outcome`, …), each with a managed
section that names the action, why it matters, what it is expected to change,
and a link back to the space. Closing an issue records that the work was
reported done; whether it had its effect is answered in the space, not by the
close.
