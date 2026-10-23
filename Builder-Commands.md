# Builder Commands

Builder inherits [regular user commands](User-Commands.md). Most builder-specific
permissions are restricted by LuckPerms to the `bigflatness2` world; they are not
a global creative or WorldEdit grant.

## World access and building mode

Configured builder nodes include teleport/rejoin access for `bigflatness2` and
`world1`, plus legacy Essentials nodes for `/back` and creative/survival game
modes. Essentials is not active, so those legacy nodes may not provide working
commands. Use CMI equivalents only if separately granted.

## WorldEdit selections

| Command | Purpose |
| --- | --- |
| `//wand` | Obtain the selection wand. |
| `//pos1`, `//pos2` | Set selection points. |
| `//hpos1`, `//hpos2` | Set points using targeted blocks. |
| `//chunk` | Select the current chunk. |
| `//expand`, `//contract` | Resize a selection. |
| `//shift`, `//outset`, `//inset` | Move or reshape a selection. |
| `//size`, `//count` | Inspect a selection. |

## WorldEdit editing and generation

Builders have region operations including set, replace, overlay, walls, faces,
smooth, naturalize, move, stack, line, curve, forest, flora, hollow, center, and
deform. They also have cylinder, sphere, pyramid, forest, pumpkin, and shape
generation permissions.

Clipboard access includes copy, cut, paste, rotate, flip, load, save, and clear.
History access includes undo, redo, and history clearing for permitted edits.
Navigation includes through, jump-to, up, ascend, descend, ceiling, and unstuck.

## WorldEdit brushes and tools

Builder permissions cover the brush system, including set, sphere, cylinder,
smooth, blend, erode, raise/lower, line, spline, scatter, surface, clipboard,
forest, gravity, snow, rock, stencil, sweep, shatter, and brush option controls.
Tree and replacer tools are also available.

`worldedit.superpickaxe`, `.area`, and `.recursive` are explicitly denied.
Large operations can lag or damage a world; make a selection carefully and use
undo immediately after a mistake. See [WorldEdit](Plugin-Guides/WorldEdit.md).

## Residence in the build world

Builders have Residence creation, bypass, ignored coordinate limits, unlimited
Residence count, and unlimited subzone permissions in `bigflatness2`. These are
construction privileges, not permission to alter unrelated player work.
