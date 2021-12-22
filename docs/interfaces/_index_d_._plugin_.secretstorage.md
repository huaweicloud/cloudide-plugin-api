**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SecretStorage

# Interface: SecretStorage

Represents a storage utility for secrets, information that is
sensitive.

## Hierarchy

* **SecretStorage**

## Index

### Properties

* [onDidChange](_index_d_._plugin_.secretstorage.md#ondidchange)

### Methods

* [delete](_index_d_._plugin_.secretstorage.md#delete)
* [get](_index_d_._plugin_.secretstorage.md#get)
* [store](_index_d_._plugin_.secretstorage.md#store)

## Properties

### onDidChange

•  **onDidChange**: [Event](_index_d_._plugin_.event.md)\<[SecretStorageChangeEvent](_index_d_._plugin_.secretstoragechangeevent.md)>

*Defined in [index.d.ts:6130](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6130)*

Fires when a secret is stored or deleted.

## Methods

### delete

▸ **delete**(`key`: string): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:6125](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6125)*

Remove a secret from storage.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`key` | string | The key the secret was stored under.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

___

### get

▸ **get**(`key`: string): [Thenable](_index_d_.thenable.md)\<string \| undefined>

*Defined in [index.d.ts:6112](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6112)*

Retrieve a secret that was stored with key. Returns undefined if there
is no password matching that key.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`key` | string | The key the secret was stored under. |

**Returns:** [Thenable](_index_d_.thenable.md)\<string \| undefined>

The stored value or `undefined`.

___

### store

▸ **store**(`key`: string, `value`: string): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:6119](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6119)*

Store a secret under a given key.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`key` | string | The key to store the secret under. |
`value` | string | The secret.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>