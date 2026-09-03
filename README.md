# loom-weave

## Card

**Just did.** Promote-then-comply rule replaced the OPEN line on the base render class.
**Next.** Receive the slot spec once it proves out in `loom-weave-godot`.
**Waiting on.** A ruling on which node carries close-out fields in a repo with no tree — this one included.

Hand-written. This repo has no `thread.json`, so `card.py` has no node
to read here. That is the open item above.

Base render contract for Loom.

Implementations live in separate repos named `loom-weave-<engine>`
(for example `loom-weave-godot`). Forking produces a new weave, not
a new tool.

No renderer code in this repo. The schema lives in `loom-warp`. Trees
live in `loom` (Loom's own) and `loom-apollo-13` (probe).

How this repo receives contracts: work happens in a weave
(`loom-weave-godot` first). When a shape proves out there, it is
promoted up into this repo as the common contract, and the weave
then conforms to what it promoted. Nothing is authored here in
advance. Ruled 2026-09-03; closes the question of where the base
render class lives. Decision node: `decisions/base-render-class`
in `loom`.
