# Project model

## System

David Joseph and Rufus Pollock. For the time being they are treated as the same
system as the 2R Research Circle (`ASM-1`, confirmed).

The 2R movement is the **environment** this system acts on. Movement-wide health
is an outcome the system aims at, not a condition it can be held to.

## Goal

`G-1` — **The 2R movement adopts LTP and benefits from it.**

Both halves carry weight. Adoption without benefit would not be worth having;
benefit without use would not be adoption. The whiteboard attaches two marginal
notes that define what "adopts" means, and they are modelled as the first two
success factors:

- `CSF-1` — a non-trivial subset of the movement is actively using LTP.
- `CSF-2` — LTP is used in shared spaces such as the forum, so that even people
  who are not "bought in" benefit from it.

`CSF-2` matters more than it looks: it means adoption cannot require everyone to
do tree work (`ASM-3`).

## Throughput

> **New users of LTP and its outputs, including people who discover 2R through
> them.**

Not papers written, meetings held, or trees edited.

This unit is contested. In July, David and Rufus agreed that the research
group's throughput is *duly improved 2R LTP trees* (`EVD-14`); the whiteboard,
later that month, states the unit above (`EVD-3`). The two are recorded as a
contradiction rather than merged. Only the tree-improvement unit currently has
any observable history, and that is what the dashboard's generated throughput
track measures.

## Above the goal

Recorded in the model but excluded from the Goal Tree view, because they lie
outside this system's control:

- `HLO-1` — A (more) effective and healthy 2R movement. The whiteboard reaches
  it from adoption through an if-then arrow.
- `LEARN-1` — The movement revises what it does in light of what the trees and
  the results show. Expanded from a one-word "Learning" box; `inferred`.
- `VIS-1` — The world thinks better and collaborates better, using trees and
  similar structure.
- `VIS-2` — We are connecting solutions to problems.

They are linked (`L-001` to `L-005`) so the chain from goal to vision is
inspectable in the YAML.

## Constraint

`IC-4` — **We have no way of committing to action.**

This is the named cause of `UDE-2` ("Rufus and David are not using LTP
consistently"), the only undesirable effect the notes marked with three flames,
and it is the point every hypothesis in the notes aims at: a transition tree
whose items are tracked in something like GitHub Issues.

## The loop that keeps it stuck

The notes do not draw this, but their own causes imply it:

```text
UDE-2  Rufus and David are not using LTP consistently
  ↓
UDE-4  The trees are not the source of truth for assessing progress
  ↓
IC-1   We do not have evidence that LTP is helping yet
  ↓
UDE-1  Nobody else is using LTP — a lack of buy-in
  ↓
(no external pressure to use it consistently)
```

`UDE-2` also causes `UDE-1` directly (`L-117`): if the two people who built the
method do not run on it, nobody else will (`ASM-2`). Nothing in this loop breaks
on its own, which is why the recommended action is inside it rather than
downstream of it.

## Views built

| View | Entities | Root(s) |
|---|---|---|
| `goal-tree` | 27 | `G-1` |
| `current-reality` | 18 | `UDE-1`, `UDE-3` |
| `transition-tree` | 18 | the eight necessary conditions the actions serve |

`evaporating-cloud`, `future-reality`, and `prerequisite-tree` are absent. The
notes' conflict-resolution section is blank, and nothing else in the sources
supports them.

## Counts

59 entities, 71 links, 17 evidence items, 9 assumptions, 10 open questions,
5 contradictions, 7 coverage gaps.
