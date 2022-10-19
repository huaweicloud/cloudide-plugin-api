[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookDocument

# Interface: NotebookDocument

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookDocument

Represents a notebook which itself is a sequence of [code or markup cells](codearts_plugin_.NotebookCell.md). Notebook documents are
created from [notebook data](../classes/codearts_plugin_.NotebookData.md).

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

The number of cells in the notebook.

#### Defined in

[index.d.ts:13214](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13214)

___

### isClosed

• `Readonly` **isClosed**: `boolean`

`true` if the notebook has been closed. A closed notebook isn't synchronized anymore
and won't be re-used when the same resource is opened again.

#### Defined in

[index.d.ts:13204](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13204)

___

### isDirty

• `Readonly` **isDirty**: `boolean`

`true` if there are unpersisted changes.

#### Defined in

[index.d.ts:13193](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13193)

___

### isUntitled

• `Readonly` **isUntitled**: `boolean`

Is this notebook representing an untitled file which has not been saved yet.

#### Defined in

[index.d.ts:13198](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13198)

___

### metadata

• `Readonly` **metadata**: `Object`

Arbitrary metadata for this notebook. Can be anything but must be JSON-stringifyable.

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

[index.d.ts:13209](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13209)

___

### notebookType

• `Readonly` **notebookType**: `string`

The type of notebook.

#### Defined in

[index.d.ts:13182](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13182)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The associated uri for this notebook.

*Note* that most notebooks use the `file`-scheme, which means they are files on disk. However, **not** all notebooks are
saved on disk and therefore the `scheme` must be checked before trying to access the underlying file or siblings on disk.

**`See`**

[FileSystemProvider](codearts_plugin_.FileSystemProvider.md)

#### Defined in

[index.d.ts:13177](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13177)

___

### version

• `Readonly` **version**: `number`

The version number of this notebook (it will strictly increase after each
change, including undo/redo).

#### Defined in

[index.d.ts:13188](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13188)

## Methods

### cellAt

▸ **cellAt**(`index`): [`NotebookCell`](codearts_plugin_.NotebookCell.md)

Return the cell at the specified index. The index will be adjusted to the notebook.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | The index of the cell to retrieve. |

#### Returns

[`NotebookCell`](codearts_plugin_.NotebookCell.md)

A [cell](codearts_plugin_.NotebookCell.md).

#### Defined in

[index.d.ts:13222](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13222)

___

### getCells

▸ **getCells**(`range?`): [`NotebookCell`](codearts_plugin_.NotebookCell.md)[]

Get the cells of this notebook. A subset can be retrieved by providing
a range. The range will be adjusted to the notebook.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range?` | [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md) | A notebook range. |

#### Returns

[`NotebookCell`](codearts_plugin_.NotebookCell.md)[]

The cells contained by the range or all cells.

#### Defined in

[index.d.ts:13231](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13231)

___

### save

▸ **save**(): [`Thenable`](Thenable.md)<`boolean`\>

Save the document. The saving will be handled by the corresponding [serializer](codearts_plugin_.NotebookSerializer.md).

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

A promise that will resolve to true when the document
has been saved. Will return false if the file was not dirty or when save failed.

#### Defined in

[index.d.ts:13239](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13239)
