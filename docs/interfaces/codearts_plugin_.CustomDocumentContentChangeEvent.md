[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomDocumentContentChangeEvent

# Interface: CustomDocumentContentChangeEvent<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomDocumentContentChangeEvent

Event triggered by extensions to signal to the editor that the content of a [`CustomDocument`](codearts_plugin_.CustomDocument.md)
has changed.

**`See`**

[`onDidChangeCustomDocument`](codearts_plugin_.CustomEditorProvider.md#ondidchangecustomdocument).

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CustomDocument`](codearts_plugin_.CustomDocument.md) = [`CustomDocument`](codearts_plugin_.CustomDocument.md) |

## Table of contents

### Properties

- [document](codearts_plugin_.CustomDocumentContentChangeEvent.md#document)

## Properties

### document

• `Readonly` **document**: `T`

The document that the change is for.

#### Defined in

[index.d.ts:8891](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L8891)
