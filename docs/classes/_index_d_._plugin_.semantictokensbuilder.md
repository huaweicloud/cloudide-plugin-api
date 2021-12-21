**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SemanticTokensBuilder

# Class: SemanticTokensBuilder

A semantic tokens builder can help with creating a `SemanticTokens` instance
which contains delta encoded semantic tokens.

## Hierarchy

* **SemanticTokensBuilder**

## Index

### Constructors

* [constructor](_index_d_._plugin_.semantictokensbuilder.md#constructor)

### Methods

* [build](_index_d_._plugin_.semantictokensbuilder.md#build)
* [push](_index_d_._plugin_.semantictokensbuilder.md#push)

## Constructors

### constructor

\+ **new SemanticTokensBuilder**(`legend?`: [SemanticTokensLegend](_index_d_._plugin_.semantictokenslegend.md)): [SemanticTokensBuilder](_index_d_._plugin_.semantictokensbuilder.md)

*Defined in [index.d.ts:3431](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3431)*

#### Parameters:

Name | Type |
------ | ------ |
`legend?` | [SemanticTokensLegend](_index_d_._plugin_.semantictokenslegend.md) |

**Returns:** [SemanticTokensBuilder](_index_d_._plugin_.semantictokensbuilder.md)

## Methods

### build

▸ **build**(`resultId?`: string): [SemanticTokens](_index_d_._plugin_.semantictokens.md)

*Defined in [index.d.ts:3458](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3458)*

Finish and create a `SemanticTokens` instance.

#### Parameters:

Name | Type |
------ | ------ |
`resultId?` | string |

**Returns:** [SemanticTokens](_index_d_._plugin_.semantictokens.md)

___

### push

▸ **push**(`line`: number, `char`: number, `length`: number, `tokenType`: number, `tokenModifiers?`: number): void

*Defined in [index.d.ts:3444](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3444)*

Add another token.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`line` | number | The token start line number (absolute value). |
`char` | number | The token start character (absolute value). |
`length` | number | The token length in characters. |
`tokenType` | number | The encoded token type. |
`tokenModifiers?` | number | The encoded token modifiers.  |

**Returns:** void

▸ **push**(`range`: [Range](_index_d_._plugin_.range.md), `tokenType`: string, `tokenModifiers?`: string[]): void

*Defined in [index.d.ts:3453](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3453)*

Add another token. Use only when providing a legend.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | The range of the token. Must be single-line. |
`tokenType` | string | The token type. |
`tokenModifiers?` | string[] | The token modifiers.  |

**Returns:** void
