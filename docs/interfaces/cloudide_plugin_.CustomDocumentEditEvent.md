[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CustomDocumentEditEvent

# Interface: CustomDocumentEditEvent<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CustomDocumentEditEvent

Event triggered by extensions to signal that an edit has occurred on an [`CustomDocument`](#CustomDocument).

**`See`**

[`CustomDocumentProvider.onDidChangeCustomDocument`](#CustomDocumentProvider.onDidChangeCustomDocument).

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CustomDocument`](cloudide_plugin_.CustomDocument.md) = [`CustomDocument`](cloudide_plugin_.CustomDocument.md) |

## Table of contents

### Properties

- [document](cloudide_plugin_.CustomDocumentEditEvent.md#document)
- [label](cloudide_plugin_.CustomDocumentEditEvent.md#label)

### Methods

- [redo](cloudide_plugin_.CustomDocumentEditEvent.md#redo)
- [undo](cloudide_plugin_.CustomDocumentEditEvent.md#undo)

## Properties

### document

• `Readonly` **document**: `T`

The document that the edit is for.

#### Defined in

[index.d.ts:3793](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3793)

___

### label

• `Optional` `Readonly` **label**: `string`

Display name describing the edit.

This will be shown to users in the UI for undo/redo operations.

#### Defined in

[index.d.ts:3818](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3818)

## Methods

### redo

▸ **redo**(): `void` \| [`Thenable`](Thenable.md)<`void`\>

Redo the edit operation.

This is invoked by Theia when the user redoes this edit. To implement `redo`, your
extension should restore the document and editor to the state they were in just after this
edit was added to Theia's internal edit stack by `onDidChangeCustomDocument`.

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:3811](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3811)

___

### undo

▸ **undo**(): `void` \| [`Thenable`](Thenable.md)<`void`\>

Undo the edit operation.

This is invoked by Theia when the user undoes this edit. To implement `undo`, your
extension should restore the document and editor to the state they were in just before this
edit was added to Theia's internal edit stack by `onDidChangeCustomDocument`.

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:3802](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3802)
