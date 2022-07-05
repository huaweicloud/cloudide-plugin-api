[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileWillCreateEvent

# Interface: FileWillCreateEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileWillCreateEvent

## Table of contents

### Properties

- [files](codearts_plugin_.FileWillCreateEvent.md#files)
- [token](codearts_plugin_.FileWillCreateEvent.md#token)

### Methods

- [waitUntil](codearts_plugin_.FileWillCreateEvent.md#waituntil)

## Properties

### files

• `Readonly` **files**: readonly [`Uri`](../classes/codearts_plugin_.Uri.md)[]

#### Defined in

[index.d.ts:11334](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L11334)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

#### Defined in

[index.d.ts:11329](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L11329)

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

[index.d.ts:11354](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L11354)

▸ **waitUntil**(`thenable`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | [`Thenable`](Thenable.md)<`any`\> |  |

#### Returns

`void`

#### Defined in

[index.d.ts:11363](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L11363)
