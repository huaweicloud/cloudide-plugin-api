[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookEditor

# Interface: NotebookEditor

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookEditor

## Table of contents

### Properties

- [notebook](codearts_plugin_.NotebookEditor.md#notebook)
- [selection](codearts_plugin_.NotebookEditor.md#selection)
- [selections](codearts_plugin_.NotebookEditor.md#selections)
- [viewColumn](codearts_plugin_.NotebookEditor.md#viewcolumn)
- [visibleRanges](codearts_plugin_.NotebookEditor.md#visibleranges)

### Methods

- [revealRange](codearts_plugin_.NotebookEditor.md#revealrange)

## Properties

### notebook

• `Readonly` **notebook**: [`NotebookDocument`](codearts_plugin_.NotebookDocument.md)

#### Defined in

[index.d.ts:12820](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12820)

___

### selection

• **selection**: [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md)

#### Defined in

[index.d.ts:12825](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12825)

___

### selections

• **selections**: readonly [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md)[]

#### Defined in

[index.d.ts:12832](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12832)

___

### viewColumn

• `Optional` `Readonly` **viewColumn**: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)

#### Defined in

[index.d.ts:12842](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12842)

___

### visibleRanges

• `Readonly` **visibleRanges**: readonly [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md)[]

#### Defined in

[index.d.ts:12837](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12837)

## Methods

### revealRange

▸ **revealRange**(`range`, `revealType?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md) |  |
| `revealType?` | [`NotebookEditorRevealType`](../enums/codearts_plugin_.NotebookEditorRevealType.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:12850](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12850)
