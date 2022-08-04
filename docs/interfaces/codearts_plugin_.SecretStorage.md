[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SecretStorage

# Interface: SecretStorage

["@codearts/plugin"](../modules/_codearts_plugin_.md).SecretStorage

## Table of contents

### Properties

- [onDidChange](codearts_plugin_.SecretStorage.md#ondidchange)

### Methods

- [delete](codearts_plugin_.SecretStorage.md#delete)
- [get](codearts_plugin_.SecretStorage.md#get)
- [store](codearts_plugin_.SecretStorage.md#store)

## Properties

### onDidChange

• **onDidChange**: [`Event`](codearts_plugin_.Event.md)<[`SecretStorageChangeEvent`](codearts_plugin_.SecretStorageChangeEvent.md)\>

#### Defined in

[index.d.ts:7054](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L7054)

## Methods

### delete

▸ **delete**(`key`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:7049](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L7049)

___

### get

▸ **get**(`key`): [`Thenable`](Thenable.md)<`undefined` \| `string`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` |  |

#### Returns

[`Thenable`](Thenable.md)<`undefined` \| `string`\>

#### Defined in

[index.d.ts:7036](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L7036)

___

### store

▸ **store**(`key`, `value`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` |  |
| `value` | `string` |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:7043](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L7043)
