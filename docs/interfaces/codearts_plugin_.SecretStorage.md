[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SecretStorage

# Interface: SecretStorage

["@codearts/plugin"](../modules/_codearts_plugin_.md).SecretStorage

Represents a storage utility for secrets, information that is
sensitive.

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

Fires when a secret is stored or deleted.

#### Defined in

[index.d.ts:7181](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7181)

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

[index.d.ts:7176](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7176)

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

[index.d.ts:7163](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7163)

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

[index.d.ts:7170](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7170)
