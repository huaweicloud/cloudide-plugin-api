[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TreeDragAndDropController

# Interface: TreeDragAndDropController<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).TreeDragAndDropController

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Properties

- [dragMimeTypes](codearts_plugin_.TreeDragAndDropController.md#dragmimetypes)
- [dropMimeTypes](codearts_plugin_.TreeDragAndDropController.md#dropmimetypes)

### Methods

- [handleDrag](codearts_plugin_.TreeDragAndDropController.md#handledrag)
- [handleDrop](codearts_plugin_.TreeDragAndDropController.md#handledrop)

## Properties

### dragMimeTypes

• `Readonly` **dragMimeTypes**: readonly `string`[]

#### Defined in

[index.d.ts:10141](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10141)

___

### dropMimeTypes

• `Readonly` **dropMimeTypes**: readonly `string`[]

#### Defined in

[index.d.ts:10133](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10133)

## Methods

### handleDrag

▸ `Optional` **handleDrag**(`source`, `dataTransfer`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | readonly `T`[] |  |
| `dataTransfer` | [`DataTransfer`](../classes/codearts_plugin_.DataTransfer.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:10159](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10159)

___

### handleDrop

▸ `Optional` **handleDrop**(`target`, `dataTransfer`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `undefined` \| `T` |  |
| `dataTransfer` | [`DataTransfer`](../classes/codearts_plugin_.DataTransfer.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:10170](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10170)
