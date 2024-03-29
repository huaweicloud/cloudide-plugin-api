[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellOutputItem

# Class: NotebookCellOutputItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellOutputItem

One representation of a [notebook output](codearts_plugin_.NotebookCellOutput.md), defined by MIME type and data.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.NotebookCellOutputItem.md#constructor)

### Properties

- [data](codearts_plugin_.NotebookCellOutputItem.md#data)
- [mime](codearts_plugin_.NotebookCellOutputItem.md#mime)

### Methods

- [error](codearts_plugin_.NotebookCellOutputItem.md#error)
- [json](codearts_plugin_.NotebookCellOutputItem.md#json)
- [stderr](codearts_plugin_.NotebookCellOutputItem.md#stderr)
- [stdout](codearts_plugin_.NotebookCellOutputItem.md#stdout)
- [text](codearts_plugin_.NotebookCellOutputItem.md#text)

## Constructors

### constructor

• **new NotebookCellOutputItem**(`data`, `mime`)

Create a new notebook cell output item.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `Uint8Array` | The value of the output item. |
| `mime` | `string` | The mime type of the output item. |

#### Defined in

[index.d.ts:14209](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14209)

## Properties

### data

• **data**: `Uint8Array`

The data of this output item. Must always be an array of unsigned 8-bit integers.

#### Defined in

[index.d.ts:14201](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14201)

___

### mime

• **mime**: `string`

The mime type which determines how the [`data`](codearts_plugin_.NotebookCellOutputItem.md#data)-property
is interpreted.

Notebooks have built-in support for certain mime-types, extensions can add support for new
types and override existing types.

#### Defined in

[index.d.ts:14196](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14196)

## Methods

### error

▸ `Static` **error**(`value`): [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

Factory function to create a `NotebookCellOutputItem` that uses
uses the `application/vnd.code.notebook.error` mime type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `Error` | An error object. |

#### Returns

[`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

A new output item object.

#### Defined in

[index.d.ts:14187](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14187)

___

### json

▸ `Static` **json**(`value`, `mime?`): [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

Factory function to create a `NotebookCellOutputItem` from
a JSON object.

*Note* that this function is not expecting "stringified JSON" but
an object that can be stringified. This function will throw an error
when the passed value cannot be JSON-stringified.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | A JSON-stringifyable value. |
| `mime?` | `string` | Optional MIME type, defaults to `application/json` |

#### Returns

[`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

A new output item object.

#### Defined in

[index.d.ts:14160](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14160)

___

### stderr

▸ `Static` **stderr**(`value`): [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

Factory function to create a `NotebookCellOutputItem` that uses
uses the `application/vnd.code.notebook.stderr` mime type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | A string. |

#### Returns

[`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

A new output item object.

#### Defined in

[index.d.ts:14178](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14178)

___

### stdout

▸ `Static` **stdout**(`value`): [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

Factory function to create a `NotebookCellOutputItem` that uses
uses the `application/vnd.code.notebook.stdout` mime type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | A string. |

#### Returns

[`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

A new output item object.

#### Defined in

[index.d.ts:14169](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14169)

___

### text

▸ `Static` **text**(`value`, `mime?`): [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

Factory function to create a `NotebookCellOutputItem` from a string.

*Note* that an UTF-8 encoder is used to create bytes for the string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | A string. |
| `mime?` | `string` | Optional MIME type, defaults to `text/plain`. |

#### Returns

[`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

A new output item object.

#### Defined in

[index.d.ts:14146](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14146)
