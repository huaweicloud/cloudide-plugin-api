[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DiagnosticCollection

# Interface: DiagnosticCollection

["@codearts/plugin"](../modules/_codearts_plugin_.md).DiagnosticCollection

## Table of contents

### Properties

- [name](codearts_plugin_.DiagnosticCollection.md#name)

### Methods

- [clear](codearts_plugin_.DiagnosticCollection.md#clear)
- [delete](codearts_plugin_.DiagnosticCollection.md#delete)
- [dispose](codearts_plugin_.DiagnosticCollection.md#dispose)
- [forEach](codearts_plugin_.DiagnosticCollection.md#foreach)
- [get](codearts_plugin_.DiagnosticCollection.md#get)
- [has](codearts_plugin_.DiagnosticCollection.md#has)
- [set](codearts_plugin_.DiagnosticCollection.md#set)

## Properties

### name

• `Readonly` **name**: `string`

#### Defined in

[index.d.ts:5998](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L5998)

## Methods

### clear

▸ **clear**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:6033](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L6033)

___

### delete

▸ **delete**(`uri`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:6027](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L6027)

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:6065](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L6065)

___

### forEach

▸ **forEach**(`callback`, `thisArg?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`uri`: [`Uri`](../classes/codearts_plugin_.Uri.md), `diagnostics`: readonly [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[], `collection`: [`DiagnosticCollection`](codearts_plugin_.DiagnosticCollection.md)) => `any` |  |
| `thisArg?` | `any` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:6041](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L6041)

___

### get

▸ **get**(`uri`): `undefined` \| readonly [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

`undefined` \| readonly [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]

#### Defined in

[index.d.ts:6050](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L6050)

___

### has

▸ **has**(`uri`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:6059](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L6059)

___

### set

▸ **set**(`uri`, `diagnostics`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `diagnostics` | `undefined` \| readonly [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[] |  |

#### Returns

`void`

#### Defined in

[index.d.ts:6007](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L6007)

▸ **set**(`entries`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `entries` | readonly [[`Uri`](../classes/codearts_plugin_.Uri.md), `undefined` \| readonly Diagnostic[]][] |  |

#### Returns

`void`

#### Defined in

[index.d.ts:6019](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L6019)
