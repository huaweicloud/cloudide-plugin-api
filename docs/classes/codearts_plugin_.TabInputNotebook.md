[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TabInputNotebook

# Class: TabInputNotebook

["@codearts/plugin"](../modules/_codearts_plugin_.md).TabInputNotebook

The tab represents a notebook.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TabInputNotebook.md#constructor)

### Properties

- [notebookType](codearts_plugin_.TabInputNotebook.md#notebooktype)
- [uri](codearts_plugin_.TabInputNotebook.md#uri)

## Constructors

### constructor

• **new TabInputNotebook**(`uri`, `notebookType`)

Constructs a new tab input for a notebook.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | The uri of the notebook. |
| `notebookType` | `string` | The type of notebook. Maps to [`NotebookDocuments's notebookType`](../interfaces/codearts_plugin_.NotebookDocument.md#notebooktype) |

#### Defined in

[index.d.ts:17079](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17079)

## Properties

### notebookType

• `Readonly` **notebookType**: `string`

The type of notebook. Maps to [`NotebookDocuments's notebookType`](../interfaces/codearts_plugin_.NotebookDocument.md#notebooktype)

#### Defined in

[index.d.ts:17073](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17073)

___

### uri

• `Readonly` **uri**: [`Uri`](codearts_plugin_.Uri.md)

The uri that the tab is representing.

#### Defined in

[index.d.ts:17069](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17069)
