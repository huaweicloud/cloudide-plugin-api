[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookDocument

# Interface: NotebookDocument

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookDocument

## Table of contents

### Properties

- [cellCount](codearts_plugin_.NotebookDocument.md#cellcount)
- [isClosed](codearts_plugin_.NotebookDocument.md#isclosed)
- [isDirty](codearts_plugin_.NotebookDocument.md#isdirty)
- [isUntitled](codearts_plugin_.NotebookDocument.md#isuntitled)
- [metadata](codearts_plugin_.NotebookDocument.md#metadata)
- [notebookType](codearts_plugin_.NotebookDocument.md#notebooktype)
- [uri](codearts_plugin_.NotebookDocument.md#uri)
- [version](codearts_plugin_.NotebookDocument.md#version)

### Methods

- [cellAt](codearts_plugin_.NotebookDocument.md#cellat)
- [getCells](codearts_plugin_.NotebookDocument.md#getcells)
- [save](codearts_plugin_.NotebookDocument.md#save)

## Properties

### cellCount

• `Readonly` **cellCount**: `number`

#### Defined in

[index.d.ts:12991](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12991)

___

### isClosed

• `Readonly` **isClosed**: `boolean`

#### Defined in

[index.d.ts:12981](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12981)

___

### isDirty

• `Readonly` **isDirty**: `boolean`

#### Defined in

[index.d.ts:12970](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12970)

___

### isUntitled

• `Readonly` **isUntitled**: `boolean`

#### Defined in

[index.d.ts:12975](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12975)

___

### metadata

• `Readonly` **metadata**: `Object`

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

[index.d.ts:12986](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12986)

___

### notebookType

• `Readonly` **notebookType**: `string`

#### Defined in

[index.d.ts:12959](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12959)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:12954](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12954)

___

### version

• `Readonly` **version**: `number`

#### Defined in

[index.d.ts:12965](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12965)

## Methods

### cellAt

▸ **cellAt**(`index`): [`NotebookCell`](codearts_plugin_.NotebookCell.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` |  |

#### Returns

[`NotebookCell`](codearts_plugin_.NotebookCell.md)

#### Defined in

[index.d.ts:12999](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12999)

___

### getCells

▸ **getCells**(`range?`): [`NotebookCell`](codearts_plugin_.NotebookCell.md)[]

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range?` | [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md) |  |

#### Returns

[`NotebookCell`](codearts_plugin_.NotebookCell.md)[]

#### Defined in

[index.d.ts:13008](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13008)

___

### save

▸ **save**(): [`Thenable`](Thenable.md)<`boolean`\>

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:13016](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13016)
