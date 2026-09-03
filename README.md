# loom-weave

<!-- card:start -->

## Card

**Just did.** Standalone operation root. Card is generated from this node.
**Next.** Receive the slot spec once it proves out in `loom-weave-godot`.

<!-- card:end -->

Base render contract for Loom.

Implementations live in separate repos named `loom-weave-<engine>`
(for example `loom-weave-godot`). Forking produces a new weave, not
a new tool.

No renderer code in this repo. The schema lives in `loom-warp`. Trees
live in `loom` (Loom's own) and `loom-apollo-13` (probe).

Tree: `thread.json` at the root, type `operation`, empty `isPartOf`.
Operations do not end. Same root shape as `loom-weave-godot`. No
child nodes here; a spec that proves out in a weave is promoted up
as prose and contract, not as a tree.

How this repo receives contracts: work happens in a weave
(`loom-weave-godot` first). When a shape proves out there, it is
promoted up into this repo as the common contract, and the weave
then conforms to what it promoted. Nothing is authored here in
advance. Ruled 2026-09-03; closes the question of where the base
render class lives. Decision node: `decisions/base-render-class`
in `loom`.
