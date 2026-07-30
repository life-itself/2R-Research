# Transition Tree

## Purpose

Turn the hypotheses already written in the problem-tree notes into executable
transitions, each with the effect it should produce and the condition it
advances.

Every action here comes from a `Hyp:` in the notes or from an explicit open
question in them. Nothing was invented to fill the tree.

Ordering is recorded on each action's `prerequisites` field rather than as links,
so the view stays a clean action → effect → condition projection:
`ACT-1` before `ACT-2` and `ACT-3`; `ACT-4` before `ACT-5`.

---

```text
Transition ID:            ACT-1  →  TR-1
Current reality:          IC-6 — no source of truth for the transition tree.
                          IC-7 — the markdown format for one is unknown.
Need:                     NC-4, NC-5 — one canonical location and a known format.
Action:                   Define a markdown format for a transition tree and
                          commit one filled-in transition tree to the 2R-Research
                          repo as its single source of truth.
Expected immediate effect: TR-1 — a canonical transition tree exists in a known
                          format and location, so an action can be written down,
                          found again, and reviewed.
Expected contribution:    NC-3 → CSF-5 → G-1. Removes the deepest cause under
                          the current constraint.
Prerequisites:            none. This is why it goes first.
Verification:             A named path holds a transition tree whose actions each
                          cite the tree entity they serve, and Rufus can read and
                          comment on it without further explanation.
Likely scope:             2R-Research — ltp/07-transition-tree.md, ltp/ltp-model.yaml
Risk:                     The format is designed once and abandoned because
                          maintaining it is more onerous than the whiteboard it
                          replaces.
Rollback:                 Text under version control; revert, or reduce to a flat
                          action list.
Traceability:             addresses IC-6, IC-7; achieves NC-4, NC-5
Confidence:               high
```

```text
Transition ID:            ACT-2  →  TR-2
Current reality:          IC-5 — no tracker for tasks and actions; tracking is verbal.
Need:                     NC-7 — actions tracked against the tree nodes they serve.
Action:                   Open GitHub Issues linked one-to-one to transition tree
                          nodes, replacing verbal tracking.
Expected immediate effect: TR-2 — every committed action has a tracked item
                          traceable to a tree node, and progress becomes visible
                          while the method is dog-fooded.
Expected contribution:    NC-3 → CSF-5 → G-1. Directly attacks IC-4.
Prerequisites:            ACT-1 — issues need tree nodes to point at.
Verification:             Every action in the transition tree has exactly one open
                          or closed issue, and each issue names its tree entity.
Likely scope:             2R-Research issues; issue references written back into
                          the transition tree.
Risk:                     Issues drift out of step with the tree and a second,
                          contradictory source of truth appears.
Rollback:                 Close the issues; the transition tree remains
                          authoritative on its own.
Traceability:             addresses IC-5; achieves NC-7, NC-3
Confidence:               high
```

```text
Transition ID:            ACT-3  →  TR-3
Current reality:          IC-8 — no way to view a transition tree.
Need:                     NC-6 — a way to view it.
Action:                   Ship a transition-tree view in the dashboard so current
                          actions can be read without opening YAML.
Expected immediate effect: TR-3 — David and Rufus can see current actions against
                          the tree, so reviewing progress does not require
                          reading the model source.
Expected contribution:    NC-4 → NC-3 → CSF-5 → G-1.
Prerequisites:            ACT-1 — the view needs a format to render.
Verification:             David and Rufus each open the dashboard and correctly
                          say what the current action is and which condition it
                          serves, without help.
Likely scope:             logical-thought-process-issue-trees-app —
                          skills/project-ltp/dashboard/src
Risk:                     Effort goes into the viewer while the underlying
                          commitments are still not being kept.
Rollback:                 The view is additive; the markdown transition tree stays
                          readable without it.
Traceability:             addresses IC-8; achieves NC-6
Confidence:               high
```

```text
Transition ID:            ACT-4  →  TR-4
Current reality:          IC-9, IC-10, IC-11 — no finalized 2R goal tree, and it
                          is undecided which trees to show and how.
Need:                     NC-12, NC-13 — something stable and presentable to
                          point at.
Action:                   Decide which 2R trees to show and how, then finalize and
                          publish that version of the 2R goal tree.
Expected immediate effect: TR-4 — one canonical, presentable 2R goal tree exists,
                          so forum posts and presented materials have something
                          stable to point at.
Expected contribution:    CSF-7 → G-1.
Prerequisites:            none formally, but see the risk: NC-1 should be settled
                          first.
Verification:             One named, dated version of the 2R goal tree is public
                          and can be linked from a forum post.
Likely scope:             2R-Research — docs/ltp_trees/; the published site
Risk:                     Finalizing unilaterally repeats the June problem, where
                          revisions from Rufus and Margaret had no agreed
                          disposition process and one person decided (EVD-15).
Rollback:                 Versions are dated, so a published version can be
                          superseded rather than deleted.
Traceability:             addresses IC-9, IC-10, IC-11; achieves NC-12, NC-13
Confidence:               medium
```

```text
Transition ID:            ACT-5  →  TR-5
Current reality:          IC-12 — no process linking the trees to forum posts, so
                          no pathway to discovering or enriching them.
Need:                     NC-14 — such a pathway.
Action:                   Link a batch of real forum and WhatsApp posts to tree
                          nodes by hand, then judge from that what is worth
                          automating.
Expected immediate effect: TR-5 — a measured manual pathway from discussion to
                          tree exists, with evidence about which part of it is
                          worth automating.
Expected contribution:    CSF-7 and CSF-8 → G-1.
Prerequisites:            ACT-4 — there must be a settled tree to map posts onto.
Verification:             A recorded batch of posts mapped to tree nodes, with the
                          time taken per post and the share of posts that map to
                          nothing.
Likely scope:             2R-Research — an annotation log; forum posts
Risk:                     Manual mapping is done once, reads as busywork, and
                          yields no decision about automation.
Rollback:                 The mapping log is an addition; nothing in the forum
                          changes.
Traceability:             addresses IC-12; achieves NC-14
Confidence:               medium
```

---

## Why the automation question is answered manually first

The notes ask "How would we automate this from e.g. whatsapp posts?" as an open
question. `ACT-5` deliberately does not answer it by building automation. The
prior attempt in this direction — the Bluesky bridge — produced suggestions that
were, by David's own account, not poignant enough, because the trees were not
mature and the matching was weak (`EVD-16`). Measuring the manual path is what
makes the automation question answerable rather than repeating that.

## What is deliberately absent

No transition addresses `IC-2` (people struggle with trees), `IC-13` (salience
and presentation), or `IC-14` (LTP is heavy duty). Those are real root causes and
they bear on `NC-15` and `NC-16`, but every available lever on them depends on
other people's behaviour, and none of them is the current constraint. They are
candidates for the next cycle, once the loop in `03-current-reality-tree.md` is
broken.
