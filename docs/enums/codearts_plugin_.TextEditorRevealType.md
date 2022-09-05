[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditorRevealType

# Enumeration: TextEditorRevealType

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditorRevealType

Represents different [reveal](../interfaces/codearts_plugin_.TextEditor.md#revealrange) strategies in a text editor.

## Table of contents

### Enumeration Members

- [AtTop](codearts_plugin_.TextEditorRevealType.md#attop)
- [Default](codearts_plugin_.TextEditorRevealType.md#default)
- [InCenter](codearts_plugin_.TextEditorRevealType.md#incenter)
- [InCenterIfOutsideViewport](codearts_plugin_.TextEditorRevealType.md#incenterifoutsideviewport)

## Enumeration Members

### AtTop

• **AtTop** = ``3``

The range will always be revealed at the top of the viewport.

#### Defined in

[index.d.ts:721](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L721)

___

### Default

• **Default** = ``0``

The range will be revealed with as little scrolling as possible.

#### Defined in

[index.d.ts:708](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L708)

___

### InCenter

• **InCenter** = ``1``

The range will always be revealed in the center of the viewport.

#### Defined in

[index.d.ts:712](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L712)

___

### InCenterIfOutsideViewport

• **InCenterIfOutsideViewport** = ``2``

If the range is outside the viewport, it will be revealed in the center of the viewport.
Otherwise, it will be revealed with as little scrolling as possible.

#### Defined in

[index.d.ts:717](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L717)
