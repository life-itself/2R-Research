# Next action

## Recommendation

**`ACT-1` — Define a markdown format for a transition tree and commit one
filled-in transition tree to the 2R-Research repo as its single source of truth.**

## Why this one

The current constraint is `IC-4`, *we have no way of committing to action*. It is
the named cause of `UDE-2`, the only undesirable effect the notes marked with
three flames, and it sits inside a loop that does not break on its own:

> Rufus and David do not use LTP consistently → the trees are not the source of
> truth for progress → no evidence accumulates that LTP helps → nobody else
> adopts it → nothing forces consistent use.

`IC-4` has two causes: no tracker (`IC-5`) and no source of truth for the
transition tree (`IC-6`, itself caused by `IC-7` and `IC-8`). Of these, the
format and location come first, because a tracker (`ACT-2`) and a viewer
(`ACT-3`) both need something canonical to point at. Doing either of those first
would mean building against a shape that does not exist yet.

It is also the cheapest action on the list, entirely inside David and Rufus's
control, and it produces the artifact that makes the other four reviewable.

## Expected immediate effect

`TR-1` — a canonical transition tree exists in a known format and location, so an
action can be written down, found again, and reviewed.

## Verification

A named path holds a transition tree whose actions each cite the tree entity they
serve, and Rufus can read and comment on it without further explanation.

## What would change this recommendation

- **If `IC-4` is not really the constraint.** The three flames are David's
  priority marking, not an observation of throughput. If the real blocker is that
  nobody outside the pair sees any reason to adopt LTP, then `NC-9` — the
  convincing story — is the constraint, and `IC-3` should be retyped as a UDE.
  David already flagged that possibility in the notes.
- **If committing to action is not what turns a tree into practice** (`ASM-4`,
  `provisional`). If David and Rufus have previously kept written commitments in
  a tracker and still drifted, the cause of `UDE-2` is elsewhere — most likely
  `IC-14`, that LTP is heavy duty and taxing — and the answer is reducing the
  method's weight, not recording actions more carefully.
- **If a transition tree already exists somewhere usable.** `IC-6` and `IC-7`
  claim it does not. If there is a working format in the `project-ltp` skill that
  simply has not been applied here, `ACT-1` shrinks to adopting it, and `ACT-2`
  becomes the first real action.

## Not recommended first, and why

- **`ACT-4`** (finalize and publish a 2R goal tree) is tempting because it is the
  visible one, but it needs `NC-1` — an agreed way to update the tree — settled
  first. Publishing a version unilaterally would repeat exactly the June problem
  that started this whole line of work (`EVD-15`).
- **`ACT-5`** (link forum posts to tree nodes) depends on `ACT-4`.
- **`ACT-3`** (ship a viewer) is the most enjoyable and the easiest to mistake
  for progress. It addresses a real cause, `IC-8`, but a viewer over an
  unspecified format is work done twice.
- **Anything aimed at `IC-2`, `IC-13`, or `IC-14`** requires other people's
  behaviour to change, and none of them is the constraint.
