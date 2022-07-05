[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileWillRenameEvent

# Interface: FileWillRenameEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileWillRenameEvent

## Table of contents

### Properties

- [files](codearts_plugin_.FileWillRenameEvent.md#files)
- [token](codearts_plugin_.FileWillRenameEvent.md#token)

### Methods

- [waitUntil](codearts_plugin_.FileWillRenameEvent.md#waituntil)

## Properties

### files

• `Readonly` **files**: readonly { `newUri`: [`Uri`](../classes/codearts_plugin_.Uri.md) ; `oldUri`: [`Uri`](../classes/codearts_plugin_.Uri.md)  }[]

#### Defined in

[index.d.ts:11454](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L11454)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

#### Defined in

[index.d.ts:11449](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L11449)

## Methods

### waitUntil

▸ **waitUntil**(`thenable`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | [`Thenable`](Thenable.md)<[`WorkspaceEdit`](../classes/codearts_plugin_.WorkspaceEdit.md)\> |  |

#### Returns

`void`

#### Defined in

[index.d.ts:11474](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L11474)

▸ **waitUntil**(`thenable`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | [`Thenable`](Thenable.md)<`any`\> |  |

#### Returns

`void`

#### Defined in

[index.d.ts:11483](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L11483)
