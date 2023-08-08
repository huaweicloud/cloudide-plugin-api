[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SemanticTokensBuilder

# Class: SemanticTokensBuilder

["@codearts/plugin"](../modules/_codearts_plugin_.md).SemanticTokensBuilder

A semantic tokens builder can help with creating a `SemanticTokens` instance
which contains delta encoded semantic tokens.

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

[index.d.ts:3740](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3740)

## Methods

### build

▸ **build**(`resultId?`): [`SemanticTokens`](codearts_plugin_.SemanticTokens.md)

Finish and create a `SemanticTokens` instance.

#### Parameters

| Name | Type |
| :------ | :------ |
| `resultId?` | `string` |

#### Returns

[`SemanticTokens`](codearts_plugin_.SemanticTokens.md)

#### Defined in

[index.d.ts:3765](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3765)

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

[index.d.ts:3751](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3751)

▸ **push**(`range`, `tokenType`, `tokenModifiers?`): `void`

Add another token. Use only when providing a legend.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The range of the token. Must be single-line. |
| `tokenType` | `string` | The token type. |
| `tokenModifiers?` | readonly `string`[] | The token modifiers. |

#### Returns

`void`

#### Defined in

[index.d.ts:3760](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3760)
