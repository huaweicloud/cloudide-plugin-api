[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Uri

# Class: Uri

["@codearts/plugin"](../modules/_codearts_plugin_.md).Uri

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Uri.md#constructor)

### Properties

- [authority](codearts_plugin_.Uri.md#authority)
- [fragment](codearts_plugin_.Uri.md#fragment)
- [fsPath](codearts_plugin_.Uri.md#fspath)
- [path](codearts_plugin_.Uri.md#path)
- [query](codearts_plugin_.Uri.md#query)
- [scheme](codearts_plugin_.Uri.md#scheme)

### Methods

- [toJSON](codearts_plugin_.Uri.md#tojson)
- [toString](codearts_plugin_.Uri.md#tostring)
- [with](codearts_plugin_.Uri.md#with)
- [file](codearts_plugin_.Uri.md#file)
- [from](codearts_plugin_.Uri.md#from)
- [joinPath](codearts_plugin_.Uri.md#joinpath)
- [parse](codearts_plugin_.Uri.md#parse)

## Constructors

### constructor

• `Private` **new Uri**(`scheme`, `authority`, `path`, `query`, `fragment`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scheme` | `string` |
| `authority` | `string` |
| `path` | `string` |
| `query` | `string` |
| `fragment` | `string` |

#### Defined in

[index.d.ts:1399](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1399)

## Properties

### authority

• `Readonly` **authority**: `string`

#### Defined in

[index.d.ts:1411](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1411)

___

### fragment

• `Readonly` **fragment**: `string`

#### Defined in

[index.d.ts:1426](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1426)

___

### fsPath

• `Readonly` **fsPath**: `string`

#### Defined in

[index.d.ts:1448](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1448)

___

### path

• `Readonly` **path**: `string`

#### Defined in

[index.d.ts:1416](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1416)

___

### query

• `Readonly` **query**: `string`

#### Defined in

[index.d.ts:1421](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1421)

___

### scheme

• `Readonly` **scheme**: `string`

#### Defined in

[index.d.ts:1405](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1405)

## Methods

### toJSON

▸ **toJSON**(): `any`

#### Returns

`any`

#### Defined in

[index.d.ts:1490](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1490)

___

### toString

▸ **toString**(`skipEncoding?`): `string`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `skipEncoding?` | `boolean` |  |

#### Returns

`string`

#### Defined in

[index.d.ts:1483](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1483)

___

### with

▸ **with**(`change`): [`Uri`](codearts_plugin_.Uri.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` |  |
| `change.authority?` | `string` | - |
| `change.fragment?` | `string` | - |
| `change.path?` | `string` | - |
| `change.query?` | `string` | - |
| `change.scheme?` | `string` | - |

#### Returns

[`Uri`](codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:1464](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1464)

___

### file

▸ `Static` **file**(`path`): [`Uri`](codearts_plugin_.Uri.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` |  |

#### Returns

[`Uri`](codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:1363](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1363)

___

### from

▸ `Static` **from**(`components`): [`Uri`](codearts_plugin_.Uri.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `components` | `Object` |  |
| `components.authority?` | `string` | - |
| `components.fragment?` | `string` | - |
| `components.path?` | `string` | - |
| `components.query?` | `string` | - |
| `components.scheme` | `string` | - |

#### Returns

[`Uri`](codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:1394](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1394)

___

### joinPath

▸ `Static` **joinPath**(`base`, ...`pathSegments`): [`Uri`](codearts_plugin_.Uri.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `base` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `...pathSegments` | `string`[] |  |

#### Returns

[`Uri`](codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:1385](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1385)

___

### parse

▸ `Static` **parse**(`value`, `strict?`): [`Uri`](codearts_plugin_.Uri.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` |  |
| `strict?` | `boolean` |  |

#### Returns

[`Uri`](codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:1338](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L1338)
