[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TabInputNotebookDiff

# Class: TabInputNotebookDiff

["@codearts/plugin"](../modules/_codearts_plugin_.md).TabInputNotebookDiff

The tabs represents two notebooks in a diff configuration.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TabInputNotebookDiff.md#constructor)

### Properties

- [modified](codearts_plugin_.TabInputNotebookDiff.md#modified)
- [notebookType](codearts_plugin_.TabInputNotebookDiff.md#notebooktype)
- [original](codearts_plugin_.TabInputNotebookDiff.md#original)

## Constructors

### constructor

• **new TabInputNotebookDiff**(`original`, `modified`, `notebookType`)

Constructs a notebook diff tab input.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `original` | [`Uri`](codearts_plugin_.Uri.md) | The uri of the original unmodified notebook. |
| `modified` | [`Uri`](codearts_plugin_.Uri.md) | The uri of the modified notebook. |
| `notebookType` | `string` | The type of notebook. Maps to [`NotebookDocuments's notebookType`](../interfaces/codearts_plugin_.NotebookDocument.md#notebooktype) |

#### Defined in

[index.d.ts:17229](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17229)

## Properties

### modified

• `Readonly` **modified**: [`Uri`](codearts_plugin_.Uri.md)

The uri of the modified notebook.

#### Defined in

[index.d.ts:17218](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17218)

___

### notebookType

• `Readonly` **notebookType**: `string`

The type of notebook. Maps to [`NotebookDocuments's notebookType`](../interfaces/codearts_plugin_.NotebookDocument.md#notebooktype)

#### Defined in

[index.d.ts:17222](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17222)

___

### original

• `Readonly` **original**: [`Uri`](codearts_plugin_.Uri.md)

The uri of the original notebook.

#### Defined in

[index.d.ts:17214](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17214)
