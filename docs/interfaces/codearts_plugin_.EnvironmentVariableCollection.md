[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / EnvironmentVariableCollection

# Interface: EnvironmentVariableCollection

["@codearts/plugin"](../modules/_codearts_plugin_.md).EnvironmentVariableCollection

## Table of contents

### Properties

- [persistent](codearts_plugin_.EnvironmentVariableCollection.md#persistent)

### Methods

- [append](codearts_plugin_.EnvironmentVariableCollection.md#append)
- [clear](codearts_plugin_.EnvironmentVariableCollection.md#clear)
- [delete](codearts_plugin_.EnvironmentVariableCollection.md#delete)
- [forEach](codearts_plugin_.EnvironmentVariableCollection.md#foreach)
- [get](codearts_plugin_.EnvironmentVariableCollection.md#get)
- [prepend](codearts_plugin_.EnvironmentVariableCollection.md#prepend)
- [replace](codearts_plugin_.EnvironmentVariableCollection.md#replace)

## Properties

### persistent

• **persistent**: `boolean`

#### Defined in

[index.d.ts:10785](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10785)

## Methods

### append

▸ **append**(`variable`, `value`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `variable` | `string` |  |
| `value` | `string` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:10807](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10807)

___

### clear

▸ **clear**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:10845](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10845)

___

### delete

▸ **delete**(`variable`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `variable` | `string` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:10840](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10840)

___

### forEach

▸ **forEach**(`callback`, `thisArg?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`variable`: `string`, `mutator`: [`EnvironmentVariableMutator`](codearts_plugin_.EnvironmentVariableMutator.md), `collection`: [`EnvironmentVariableCollection`](codearts_plugin_.EnvironmentVariableCollection.md)) => `any` |  |
| `thisArg?` | `any` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:10833](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10833)

___

### get

▸ **get**(`variable`): `undefined` \| [`EnvironmentVariableMutator`](codearts_plugin_.EnvironmentVariableMutator.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `variable` | `string` |  |

#### Returns

`undefined` \| [`EnvironmentVariableMutator`](codearts_plugin_.EnvironmentVariableMutator.md)

#### Defined in

[index.d.ts:10825](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10825)

___

### prepend

▸ **prepend**(`variable`, `value`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `variable` | `string` |  |
| `value` | `string` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:10818](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10818)

___

### replace

▸ **replace**(`variable`, `value`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `variable` | `string` |  |
| `value` | `string` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:10796](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10796)
