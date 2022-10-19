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

[index.d.ts:13030](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13030)

___

### Default

• **Default** = ``0``

The range will be revealed with as little scrolling as possible.

#### Defined in

[index.d.ts:13014](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13014)

___

### InCenter

• **InCenter** = ``1``

The range will always be revealed in the center of the viewport.

#### Defined in

[index.d.ts:13019](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13019)

___

### InCenterIfOutsideViewport

• **InCenterIfOutsideViewport** = ``2``

If the range is outside the viewport, it will be revealed in the center of the viewport.
Otherwise, it will be revealed with as little scrolling as possible.

#### Defined in

[index.d.ts:13025](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13025)
