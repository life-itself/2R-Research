# Current Reality Tree

## Purpose

Explain why the necessary conditions in the Goal Tree are not satisfied — why
LTP is not being used, starting with by the two people who built it.

This tree is a direct transcription of `docs/notes/2026-07-30-problem-tree-notes.txt`,
restructured only where the notes' own labels were inconsistent with the causal
shape they describe.

## Undesirable Effects

- **UDE-1** — Nobody except Rufus and David is using LTP, so there is a lack of
  buy-in for it.
- **UDE-2** — Rufus and David are not using LTP consistently. **Three flames in
  the notes: the highest priority of the four.**
- **UDE-3** — LTP results and outputs are not showing up where the movement
  works, such as the forum and our presented materials.
- **UDE-4** — The trees are not being used as a source of truth for assessing
  progress and learning.

All four are `observed`, high confidence.

## Causes

Under `UDE-1`:

- **IC-1** — We do not have evidence that LTP is helping yet. *(intermediate —
  it has a cause of its own, see the loop below)*
- **IC-2** — People struggle with trees, structured thinking, and complexity.
  *(intermediate — caused by `IC-14`)*
- **IC-3** — We do not have a convincing story of how or where LTP would help.
  One flame. David's own note says this could be a UDE rather than a cause.

Under `UDE-2`, the fullest chain in the notes:

- **IC-4** — We have no way of committing to action. **← current constraint**
  - **IC-5** — We have no tracker for tasks and actions.
  - **IC-6** — We have no source of truth for the transition tree.
    - **IC-7** — We do not know the format for a transition tree in markdown.
    - **IC-8** — We have no way to view a transition tree.

Under `UDE-3`:

- **IC-9** — We have not finalized a 2R goal tree.
  - **IC-10** — It is not decided which trees we want to show.
  - **IC-11** — It is not decided how to present the trees usefully.
- **IC-12** — We have no automated process linking the trees to forum posts, so
  there is no pathway to discovering or enriching them.

Common to several effects, as the notes' own final section says:

- **IC-13** — The most salient information is not presented to the viewer when
  they look at a tree, for example on our website. The notes' footnote calls this
  "a UX IC behind several other items", so it is modelled as a cause of `UDE-1`,
  `UDE-4`, and `IC-11`.
- **IC-14** — LTP is heavy duty, complex, and taxing. A cause of `IC-2` and a
  contributor to `UDE-2`.

## The reinforcing loop

The notes list `UDE-2` and `UDE-4` separately and give `UDE-4` no causes. Reading
their content together produces a loop that none of the four effects escapes:

```text
UDE-2  Rufus and David are not using LTP consistently   (L-119)
  ↓
UDE-4  The trees are not the source of truth for progress   (L-120)
  ↓
IC-1   We do not have evidence that LTP is helping yet   (L-100)
  ↓
UDE-1  Nobody else is using LTP — lack of buy-in
```

Plus `UDE-2 → UDE-1` directly (`L-117`), on the assumption that if the method's
authors do not run on it, nobody else will (`ASM-2`), and `UDE-2 → UDE-3`
(`L-118`).

Causality reading:

> If the trees are not used to assess progress, then no evidence accumulates
> that LTP helps, because the only evidence available would be the record of
> using it (`ASM-6`).

This is why "get evidence it works" cannot be sequenced before "use it": the
evidence is a by-product of use. It is also recorded as a contradiction — `IC-1`
is given as a cause of low buy-in, but it is downstream of `UDE-4`, so neither
is prior.

## Structural corrections made

- `IC-1` and `IC-2` are labelled intermediate, not root, causes. The notes list
  them as leaves, but `IC-1` is caused by `UDE-4` and `IC-2` by `IC-14`.
- `IC-11` is intermediate, not a leaf: the notes' own aside "(similar to UDE
  below)" points at `IC-13`, which is modelled as its cause.
- Root causes, with nothing beneath them: `IC-3`, `IC-5`, `IC-7`, `IC-8`,
  `IC-10`, `IC-12`, `IC-13`, `IC-14`.

## Why `IC-4` is the constraint

- It is the named cause of the only three-flame effect.
- It sits inside the reinforcing loop, not downstream of it.
- Every hypothesis the notes attach to a cause aims at it: a transition tree,
  tracked in a tracker, held in the repo, with a way to view it.
- Its own causes (`IC-5` to `IC-8`) are small, concrete, and entirely within
  David and Rufus's control — unlike `IC-2`, `IC-13`, or `IC-14`, which need
  other people's behaviour to change.

## Roots of this view

`UDE-1` and `UDE-3`. `UDE-2` and `UDE-4` are not roots because each causes
another effect — correct causally, though it does place the three-flame effect
one level in from the top of the tree.
