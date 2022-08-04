[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomDocumentEditEvent

# Interface: CustomDocumentEditEvent<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomDocumentEditEvent

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

#### Defined in

[index.d.ts:8717](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8717)

___

### label

• `Optional` `Readonly` **label**: `string`

#### Defined in

[index.d.ts:8742](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8742)

## Methods

### redo

▸ **redo**(): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8735](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8735)

___

### undo

▸ **undo**(): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8726](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8726)
