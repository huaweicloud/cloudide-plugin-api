[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SecretStorage

# Interface: SecretStorage

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SecretStorage

Represents a storage utility for secrets, information that is
sensitive.

## Table of contents

### Properties

- [onDidChange](cloudide_plugin_.SecretStorage.md#ondidchange)

### Methods

- [delete](cloudide_plugin_.SecretStorage.md#delete)
- [get](cloudide_plugin_.SecretStorage.md#get)
- [store](cloudide_plugin_.SecretStorage.md#store)

## Properties

### onDidChange

• **onDidChange**: [`Event`](cloudide_plugin_.Event.md)<[`SecretStorageChangeEvent`](cloudide_plugin_.SecretStorageChangeEvent.md)\>

Fires when a secret is stored or deleted.

#### Defined in

[index.d.ts:3353](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3353)

## Methods

### delete

▸ **delete**(`key`): [`Thenable`](Thenable.md)<`void`\>

Remove a secret from storage.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | The key the secret was stored under. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:3348](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3348)

___

### get

▸ **get**(`key`): [`Thenable`](Thenable.md)<`undefined` \| `string`\>

Retrieve a secret that was stored with key. Returns undefined if there
is no password matching that key.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | The key the secret was stored under. |

#### Returns

[`Thenable`](Thenable.md)<`undefined` \| `string`\>

The stored value or `undefined`.

#### Defined in

[index.d.ts:3335](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3335)

___

### store

▸ **store**(`key`, `value`): [`Thenable`](Thenable.md)<`void`\>

Store a secret under a given key.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | The key to store the secret under. |
| `value` | `string` | The secret. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:3342](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3342)
