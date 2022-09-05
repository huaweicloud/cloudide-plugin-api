[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Memento

# Interface: Memento

["@codearts/plugin"](../modules/_codearts_plugin_.md).Memento

A memento represents a storage utility. It can store and retrieve
values.

## Table of contents

### Methods

- [get](codearts_plugin_.Memento.md#get)
- [keys](codearts_plugin_.Memento.md#keys)
- [update](codearts_plugin_.Memento.md#update)

## Methods

### get

▸ **get**<`T`\>(`key`): `undefined` \| `T`

Return a value.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | A string. |

#### Returns

`undefined` \| `T`

The stored value or `undefined`.

#### Defined in

[index.d.ts:6991](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6991)

▸ **get**<`T`\>(`key`, `defaultValue`): `T`

Return a value.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | A string. |
| `defaultValue` | `T` | A value that should be returned when there is no value (`undefined`) with the given key. |

#### Returns

`T`

The stored value or the defaultValue.

#### Defined in

[index.d.ts:7001](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7001)

___

### keys

▸ **keys**(): readonly `string`[]

Returns the stored keys.

#### Returns

readonly `string`[]

The stored keys.

#### Defined in

[index.d.ts:6983](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6983)

___

### update

▸ **update**(`key`, `value`): [`Thenable`](Thenable.md)<`void`\>

Store a value. The value must be JSON-stringifyable.

*Note* that using `undefined` as value removes the key from the underlying
storage.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | A string. |
| `value` | `any` | A value. MUST not contain cyclic references. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:7012](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7012)
