**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SemanticTokensLegend

# Class: SemanticTokensLegend

A semantic tokens legend contains the needed information to decipher
the integer encoded representation of semantic tokens.

## Hierarchy

* **SemanticTokensLegend**

## Index

### Constructors

* [constructor](_index_d_._plugin_.semantictokenslegend.md#constructor)

### Properties

* [tokenModifiers](_index_d_._plugin_.semantictokenslegend.md#tokenmodifiers)
* [tokenTypes](_index_d_._plugin_.semantictokenslegend.md#tokentypes)

## Constructors

### constructor

\+ **new SemanticTokensLegend**(`tokenTypes`: string[], `tokenModifiers?`: string[]): [SemanticTokensLegend](_index_d_._plugin_.semantictokenslegend.md)

*Defined in [index.d.ts:3422](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3422)*

#### Parameters:

Name | Type |
------ | ------ |
`tokenTypes` | string[] |
`tokenModifiers?` | string[] |

**Returns:** [SemanticTokensLegend](_index_d_._plugin_.semantictokenslegend.md)

## Properties

### tokenModifiers

• `Readonly` **tokenModifiers**: string[]

*Defined in [index.d.ts:3422](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3422)*

The possible token modifiers.

___

### tokenTypes

• `Readonly` **tokenTypes**: string[]

*Defined in [index.d.ts:3418](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3418)*

The possible token types.
