[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellOutput

# Class: NotebookCellOutput

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellOutput

Notebook cell output represents a result of executing a cell. It is a container type for multiple
[output items](codearts_plugin_.NotebookCellOutputItem.md) where contained items represent the same result but
use different MIME types.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.NotebookCellOutput.md#constructor)

### Properties

- [items](codearts_plugin_.NotebookCellOutput.md#items)
- [metadata](codearts_plugin_.NotebookCellOutput.md#metadata)

## Constructors

### constructor

• **new NotebookCellOutput**(`items`, `metadata?`)

Create new notebook output.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)[] | Notebook output items. |
| `metadata?` | `Object` | Optional metadata. |

#### Defined in

[index.d.ts:13343](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13343)

## Properties

### items

• **items**: [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)[]

The output items of this output. Each item must represent the same result. _Note_ that repeated
MIME types per output is invalid and that the editor will just pick one of them.

```ts
new vscode.NotebookCellOutput([
	vscode.NotebookCellOutputItem.text('Hello', 'text/plain'),
	vscode.NotebookCellOutputItem.text('<i>Hello</i>', 'text/html'),
	vscode.NotebookCellOutputItem.text('_Hello_', 'text/markdown'),
	vscode.NotebookCellOutputItem.text('Hey', 'text/plain'), // INVALID: repeated type, editor will pick just one
])
```

#### Defined in

[index.d.ts:13330](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13330)

___

### metadata

• `Optional` **metadata**: `Object`

Arbitrary metadata for this cell output. Can be anything but must be JSON-stringifyable.

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

[index.d.ts:13335](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13335)
