# Coverage and evidence

## Scope

This analysis models **David Joseph and Rufus Pollock**, treated for the time
being as the same system as the 2R Research Circle. The 2R movement is the
environment this system acts on, not part of the system.

It replaces an earlier analysis that took the Research Circle's inquiry process
as the system and named missing revision governance as the constraint. That
model was rebuilt, not amended, because its goal and its constraint did not
match the account David and Rufus give of their own situation.

Primary sources, both from July 2026 and both supplied by David:

- `docs/notes/2026-07-30-problem-tree-notes.txt` — a hand-written problem tree:
  four undesirable effects, their causes, hypotheses attached to several of
  those causes, and an unfinished conflict-resolution section.
- `docs/notes/2026-07-24-goal-and-throughput-whiteboard.png`, with the
  transcription `docs/notes/2026-07-24-goal-and-throughput-whiteboard.md` — a
  whiteboard answering "What is David and Rufus' goal and throughput?". It
  holds two vision boxes, a goal with two marginal definitions of adoption, a
  throughput definition, a results axis, and two clusters of success factors.

Supporting sources:

- `docs/prompts/LTP_BACKGROUND_PROMPT.md` — background narrative and two quoted
  exchanges, one with RobertBunge on the forum and one with Rufus about
  throughput.
- `docs/ltp_trees/*.md` — the five pre-existing 2R trees.

## Classification

| Files | Category | Treatment |
|---|---|---|
| 2 primary notes (+ 1 transcription) | Participants' own trees and definitions | Authoritative; read in full |
| 1 background prompt | Project framing and participant dialogue | Examined directly, cited where it bears on the notes |
| 5 pre-existing 2R trees | Prior organization-level model | Cited as context; not re-analysed |

The notes are authoritative for this system's goal, throughput, undesirable
effects, and causes, because they are the participants' own statements rather
than an interpretation of them. Entities taken directly from the notes carry
status `confirmed` or `observed`. Where a statement was restructured, expanded,
or inverted into a condition, the entity carries `inferred` or `provisional` and
says so in its `reasoning` field.

The pre-existing 2R trees describe 2R proper. Their claims were not imported as
facts about this system.

## Evidence map

17 evidence items, `EVD-1` to `EVD-17`:

| Range | Source | Covers |
|---|---|---|
| EVD-1 – EVD-7 | Whiteboard transcription | Visions, the goal and its two adoption tests, throughput, results, both CSF clusters |
| EVD-8 – EVD-13 | Problem-tree notes | Four UDEs, their cause chains, the two common causes, the empty conflict stub |
| EVD-14 – EVD-16 | Background prompt | The July throughput agreement, the June revision-governance problem, the Bluesky and empty-dancefloor experiment |
| EVD-17 | `docs/ltp_trees/Goal Tree_ Second Renaissance.md` | The draft 2R goal tree that "not finalized" refers to |

Every entity cites at least one evidence item. `EVD-13` is cited by no entity by
design: it records that the notes' conflict-resolution section is blank, which
justifies a coverage gap rather than a claim.

## What was not covered

- The notes' **Conflict Resolution** section is an empty stub (`EVD-13`). No
  Evaporating Cloud, Future Reality Tree, or Prerequisite Tree was built.
  `04-evaporating-clouds.md`, `05-future-reality-tree.md`, and
  `06-prerequisite-tree.md` were **removed** rather than left standing on the
  superseded analysis.
- No forum export, WhatsApp export, or website analytics was supplied, so the
  claims about forum use and about discoverability rest on the notes alone.
- No funding target, budget, or funder conversation was supplied, so `CSF-9`
  has nothing beneath it except agreement on needs and offers.
- No history exists for "new users of LTP and its outputs", so no throughput
  file was authored for that unit. The dashboard's throughput track for this
  project measures the other candidate unit — adopted changes to the shared 2R
  model, derived from Git history — and is generated, not authored.
- UDE-3 and UDE-4 rest on one line each in the notes, with no independent
  observation behind them.
- The whiteboard's "Learning" and "Results" axis labels were transcribed in full
  but only partly interpreted. `LEARN-1` is an expansion of a one-word box.

## Validation performed

- Parsed `ltp-model.yaml` and validated it against
  `references/ltp-model.schema.json`.
- Checked that entity and link IDs are unique, that every link endpoint exists,
  and that every ID named in a view exists.
- Checked that both endpoints of every view link are themselves in that view.
- Checked that every cited evidence and assumption ID resolves, and that
  `analysis.current_constraint`, `recommended_next_action`, `expected_effect`,
  and `project.provisional_goal` all resolve.
- Checked that no entity typed `root_cause` has causes beneath it. Two did on
  the first pass, `IC-1` and `IC-2`; both were retyped `intermediate_cause`.
- Confirmed the Goal Tree has a single root, `G-1`.
- Rendered all three views in the dashboard and confirmed the removed views
  appear as unavailable rather than as empty trees.
