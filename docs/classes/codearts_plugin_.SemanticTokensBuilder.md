[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SemanticTokensBuilder

# Class: SemanticTokensBuilder

["@codearts/plugin"](../modules/_codearts_plugin_.md).SemanticTokensBuilder

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SemanticTokensBuilder.md#constructor)

### Methods

- [build](codearts_plugin_.SemanticTokensBuilder.md#build)
- [push](codearts_plugin_.SemanticTokensBuilder.md#push)

## Constructors

### constructor

• **new SemanticTokensBuilder**(`legend?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `legend?` | [`SemanticTokensLegend`](codearts_plugin_.SemanticTokensLegend.md) |

#### Defined in

[index.d.ts:3702](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L3702)

## Methods

### build

▸ **build**(`resultId?`): [`SemanticTokens`](codearts_plugin_.SemanticTokens.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `resultId?` | `string` |

#### Returns

[`SemanticTokens`](codearts_plugin_.SemanticTokens.md)

#### Defined in

[index.d.ts:3727](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L3727)

___

### push

▸ **push**(`line`, `char`, `length`, `tokenType`, `tokenModifiers?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `line` | `number` |  |
| `char` | `number` |  |
| `length` | `number` |  |
| `tokenType` | `number` |  |
| `tokenModifiers?` | `number` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:3713](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L3713)

▸ **push**(`range`, `tokenType`, `tokenModifiers?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |
| `tokenType` | `string` |  |
| `tokenModifiers?` | readonly `string`[] |  |

#### Returns

`void`

#### Defined in

[index.d.ts:3722](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L3722)
