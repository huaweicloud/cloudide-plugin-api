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

[index.d.ts:10815](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10815)

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

[index.d.ts:10837](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10837)

___

### clear

▸ **clear**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:10875](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10875)

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

[index.d.ts:10870](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10870)

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

[index.d.ts:10863](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10863)

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

[index.d.ts:10855](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10855)

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

[index.d.ts:10848](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10848)

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

[index.d.ts:10826](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10826)
