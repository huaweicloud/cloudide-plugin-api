[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileWillDeleteEvent

# Interface: FileWillDeleteEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileWillDeleteEvent

## Table of contents

### Properties

- [files](codearts_plugin_.FileWillDeleteEvent.md#files)
- [token](codearts_plugin_.FileWillDeleteEvent.md#token)

### Methods

- [waitUntil](codearts_plugin_.FileWillDeleteEvent.md#waituntil)

## Properties

### files

• `Readonly` **files**: readonly [`Uri`](../classes/codearts_plugin_.Uri.md)[]

#### Defined in

[index.d.ts:11424](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11424)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

#### Defined in

[index.d.ts:11419](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11419)

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

[index.d.ts:11444](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11444)

▸ **waitUntil**(`thenable`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | [`Thenable`](Thenable.md)<`any`\> |  |

#### Returns

`void`

#### Defined in

[index.d.ts:11453](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11453)
