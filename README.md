# loom-weave

Base render contract for Loom.

Implementations live in separate repos named `loom-weave-<engine>`
(for example `loom-weave-godot`). Forking produces a new weave, not
a new tool.

No renderer code in this repo. The schema lives in `loom-warp`. Trees
live in `loom` (Loom's own) and `loom-apollo-13` (probe).

Where the base render class lives (warp vs this repo) is OPEN.
