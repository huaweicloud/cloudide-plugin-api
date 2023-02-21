[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Memento

# Interface: Memento

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Memento

A memento represents a storage utility. It can store and retrieve
values.

## Table of contents

### Methods

- [get](cloudide_plugin_.Memento.md#get)
- [update](cloudide_plugin_.Memento.md#update)

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

[index.d.ts:3293](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3293)

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

[index.d.ts:3303](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3303)

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

[index.d.ts:10742](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10742)

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

[index.d.ts:10752](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10752)

___

### update

▸ **update**(`key`, `value`): `PromiseLike`<`void`\>

Store a value. The value must be JSON-stringifyable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | A string. |
| `value` | `any` | A value. MUST not contain cyclic references. |

#### Returns

`PromiseLike`<`void`\>

#### Defined in

[index.d.ts:3311](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3311)

▸ **update**(`key`, `value`): `PromiseLike`<`void`\>

Store a value. The value must be JSON-stringifyable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | A string. |
| `value` | `any` | A value. MUST not contain cyclic references. |

#### Returns

`PromiseLike`<`void`\>

#### Defined in

[index.d.ts:10760](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10760)
