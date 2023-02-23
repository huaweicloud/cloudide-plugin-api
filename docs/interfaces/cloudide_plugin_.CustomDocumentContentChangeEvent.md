[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CustomDocumentContentChangeEvent

# Interface: CustomDocumentContentChangeEvent<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CustomDocumentContentChangeEvent

Event triggered by extensions to signal to Theia that the content of a [`CustomDocument`](#CustomDocument)
has changed.

**`See`**

[`CustomDocumentProvider.onDidChangeCustomDocument`](#CustomDocumentProvider.onDidChangeCustomDocument).

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CustomDocument`](cloudide_plugin_.CustomDocument.md) = [`CustomDocument`](cloudide_plugin_.CustomDocument.md) |

## Table of contents

### Properties

- [document](cloudide_plugin_.CustomDocumentContentChangeEvent.md#document)

## Properties

### document

• `Readonly` **document**: `T`

The document that the change is for.

#### Defined in

[index.d.ts:3831](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3831)
