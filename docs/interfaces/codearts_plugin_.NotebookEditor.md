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

[index.d.ts:12790](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L12790)

___

### selection

• **selection**: [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md)

#### Defined in

[index.d.ts:12795](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L12795)

___

### selections

• **selections**: readonly [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md)[]

#### Defined in

[index.d.ts:12802](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L12802)

___

### viewColumn

• `Optional` `Readonly` **viewColumn**: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)

#### Defined in

[index.d.ts:12812](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L12812)

___

### visibleRanges

• `Readonly` **visibleRanges**: readonly [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md)[]

#### Defined in

[index.d.ts:12807](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L12807)

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

[index.d.ts:12820](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L12820)
