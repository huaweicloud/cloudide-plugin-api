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

[index.d.ts:12961](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12961)

___

### isClosed

• `Readonly` **isClosed**: `boolean`

#### Defined in

[index.d.ts:12951](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12951)

___

### isDirty

• `Readonly` **isDirty**: `boolean`

#### Defined in

[index.d.ts:12940](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12940)

___

### isUntitled

• `Readonly` **isUntitled**: `boolean`

#### Defined in

[index.d.ts:12945](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12945)

___

### metadata

• `Readonly` **metadata**: `Object`

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

[index.d.ts:12956](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12956)

___

### notebookType

• `Readonly` **notebookType**: `string`

#### Defined in

[index.d.ts:12929](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12929)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:12924](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12924)

___

### version

• `Readonly` **version**: `number`

#### Defined in

[index.d.ts:12935](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12935)

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

[index.d.ts:12969](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12969)

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

[index.d.ts:12978](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12978)

___

### save

▸ **save**(): [`Thenable`](Thenable.md)<`boolean`\>

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:12986](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12986)
