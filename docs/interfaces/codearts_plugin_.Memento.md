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

[index.d.ts:7016](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7016)

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

[index.d.ts:7026](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7026)

___

### keys

▸ **keys**(): readonly `string`[]

Returns the stored keys.

#### Returns

readonly `string`[]

The stored keys.

#### Defined in

[index.d.ts:7008](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7008)

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

[index.d.ts:7037](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7037)
