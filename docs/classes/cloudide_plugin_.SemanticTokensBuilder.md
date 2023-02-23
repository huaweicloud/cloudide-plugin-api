[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SemanticTokensBuilder

# Class: SemanticTokensBuilder

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SemanticTokensBuilder

A semantic tokens builder can help with creating a `SemanticTokens` instance
which contains delta encoded semantic tokens.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.SemanticTokensBuilder.md#constructor)

### Methods

- [build](cloudide_plugin_.SemanticTokensBuilder.md#build)
- [push](cloudide_plugin_.SemanticTokensBuilder.md#push)

## Constructors

### constructor

• **new SemanticTokensBuilder**(`legend?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `legend?` | [`SemanticTokensLegend`](cloudide_plugin_.SemanticTokensLegend.md) |

#### Defined in

[index.d.ts:8557](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8557)

## Methods

### build

▸ **build**(`resultId?`): [`SemanticTokens`](cloudide_plugin_.SemanticTokens.md)

Finish and create a `SemanticTokens` instance.

#### Parameters

| Name | Type |
| :------ | :------ |
| `resultId?` | `string` |

#### Returns

[`SemanticTokens`](cloudide_plugin_.SemanticTokens.md)

#### Defined in

[index.d.ts:8582](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8582)

___

### push

▸ **push**(`line`, `char`, `length`, `tokenType`, `tokenModifiers?`): `void`

Add another token.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `line` | `number` | The token start line number (absolute value). |
| `char` | `number` | The token start character (absolute value). |
| `length` | `number` | The token length in characters. |
| `tokenType` | `number` | The encoded token type. |
| `tokenModifiers?` | `number` | The encoded token modifiers. |

#### Returns

`void`

#### Defined in

[index.d.ts:8568](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8568)

▸ **push**(`range`, `tokenType`, `tokenModifiers?`): `void`

Add another token. Use only when providing a legend.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | The range of the token. Must be single-line. |
| `tokenType` | `string` | The token type. |
| `tokenModifiers?` | `string`[] | The token modifiers. |

#### Returns

`void`

#### Defined in

[index.d.ts:8577](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8577)
