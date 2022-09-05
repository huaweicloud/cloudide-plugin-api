[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomDocumentEditEvent

# Interface: CustomDocumentEditEvent<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomDocumentEditEvent

Event triggered by extensions to signal to the editor that an edit has occurred on an [`CustomDocument`](codearts_plugin_.CustomDocument.md).

**`See`**

[`onDidChangeCustomDocument`](codearts_plugin_.CustomEditorProvider.md#ondidchangecustomdocument).

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CustomDocument`](codearts_plugin_.CustomDocument.md) = [`CustomDocument`](codearts_plugin_.CustomDocument.md) |

## Table of contents

### Properties

- [document](codearts_plugin_.CustomDocumentEditEvent.md#document)
- [label](codearts_plugin_.CustomDocumentEditEvent.md#label)

### Methods

- [redo](codearts_plugin_.CustomDocumentEditEvent.md#redo)
- [undo](codearts_plugin_.CustomDocumentEditEvent.md#undo)

## Properties

### document

• `Readonly` **document**: `T`

The document that the edit is for.

#### Defined in

[index.d.ts:8717](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8717)

___

### label

• `Optional` `Readonly` **label**: `string`

Display name describing the edit.

This will be shown to users in the UI for undo/redo operations.

#### Defined in

[index.d.ts:8742](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8742)

## Methods

### redo

▸ **redo**(): `void` \| [`Thenable`](Thenable.md)<`void`\>

Redo the edit operation.

This is invoked by the editor when the user redoes this edit. To implement `redo`, your
extension should restore the document and editor to the state they were in just after this
edit was added to the editor's internal edit stack by `onDidChangeCustomDocument`.

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8735](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8735)

___

### undo

▸ **undo**(): `void` \| [`Thenable`](Thenable.md)<`void`\>

Undo the edit operation.

This is invoked by the editor when the user undoes this edit. To implement `undo`, your
extension should restore the document and editor to the state they were in just before this
edit was added to the editor's internal edit stack by `onDidChangeCustomDocument`.

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8726](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8726)
