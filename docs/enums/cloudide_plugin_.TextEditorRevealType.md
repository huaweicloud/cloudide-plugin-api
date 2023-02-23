[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextEditorRevealType

# Enumeration: TextEditorRevealType

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextEditorRevealType

Represents different [reveal](#TextEditor.revealRange) strategies in a text editor.

## Table of contents

### Enumeration Members

- [AtTop](cloudide_plugin_.TextEditorRevealType.md#attop)
- [Default](cloudide_plugin_.TextEditorRevealType.md#default)
- [InCenter](cloudide_plugin_.TextEditorRevealType.md#incenter)
- [InCenterIfOutsideViewport](cloudide_plugin_.TextEditorRevealType.md#incenterifoutsideviewport)

## Enumeration Members

### AtTop

• **AtTop** = ``3``

The range will always be revealed at the top of the viewport.

#### Defined in

[index.d.ts:1157](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1157)

___

### Default

• **Default** = ``0``

The range will be revealed with as little scrolling as possible.

#### Defined in

[index.d.ts:1144](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1144)

___

### InCenter

• **InCenter** = ``1``

The range will always be revealed in the center of the viewport.

#### Defined in

[index.d.ts:1148](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1148)

___

### InCenterIfOutsideViewport

• **InCenterIfOutsideViewport** = ``2``

If the range is outside the viewport, it will be revealed in the center of the viewport.
Otherwise, it will be revealed with as little scrolling as possible.

#### Defined in

[index.d.ts:1153](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1153)
