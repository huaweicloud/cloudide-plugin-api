[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Memento

# Interface: Memento

["@codearts/plugin"](../modules/_codearts_plugin_.md).Memento

## Table of contents

### Methods

- [get](codearts_plugin_.Memento.md#get)
- [keys](codearts_plugin_.Memento.md#keys)
- [update](codearts_plugin_.Memento.md#update)

## Methods

### get

▸ **get**<`T`\>(`key`): `undefined` \| `T`

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` |  |

#### Returns

`undefined` \| `T`

#### Defined in

[index.d.ts:6991](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L6991)

▸ **get**<`T`\>(`key`, `defaultValue`): `T`

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` |  |
| `defaultValue` | `T` |  |

#### Returns

`T`

#### Defined in

[index.d.ts:7001](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7001)

___

### keys

▸ **keys**(): readonly `string`[]

#### Returns

readonly `string`[]

#### Defined in

[index.d.ts:6983](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L6983)

___

### update

▸ **update**(`key`, `value`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` |  |
| `value` | `any` |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:7012](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7012)
