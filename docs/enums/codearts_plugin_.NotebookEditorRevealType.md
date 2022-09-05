[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookEditorRevealType

# Enumeration: NotebookEditorRevealType

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookEditorRevealType

Represents a notebook editor that is attached to a [notebook](../interfaces/codearts_plugin_.NotebookDocument.md).

## Table of contents

### Enumeration Members

- [AtTop](codearts_plugin_.NotebookEditorRevealType.md#attop)
- [Default](codearts_plugin_.NotebookEditorRevealType.md#default)
- [InCenter](codearts_plugin_.NotebookEditorRevealType.md#incenter)
- [InCenterIfOutsideViewport](codearts_plugin_.NotebookEditorRevealType.md#incenterifoutsideviewport)

## Enumeration Members

### AtTop

• **AtTop** = ``3``

The range will always be revealed at the top of the viewport.

#### Defined in

[index.d.ts:12869](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L12869)

___

### Default

• **Default** = ``0``

The range will be revealed with as little scrolling as possible.

#### Defined in

[index.d.ts:12853](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L12853)

___

### InCenter

• **InCenter** = ``1``

The range will always be revealed in the center of the viewport.

#### Defined in

[index.d.ts:12858](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L12858)

___

### InCenterIfOutsideViewport

• **InCenterIfOutsideViewport** = ``2``

If the range is outside the viewport, it will be revealed in the center of the viewport.
Otherwise, it will be revealed with as little scrolling as possible.

#### Defined in

[index.d.ts:12864](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L12864)
