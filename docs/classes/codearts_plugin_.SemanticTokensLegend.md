[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SemanticTokensLegend

# Class: SemanticTokensLegend

["@codearts/plugin"](../modules/_codearts_plugin_.md).SemanticTokensLegend

A semantic tokens legend contains the needed information to decipher
the integer encoded representation of semantic tokens.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SemanticTokensLegend.md#constructor)

### Properties

- [tokenModifiers](codearts_plugin_.SemanticTokensLegend.md#tokenmodifiers)
- [tokenTypes](codearts_plugin_.SemanticTokensLegend.md#tokentypes)

## Constructors

### constructor

• **new SemanticTokensLegend**(`tokenTypes`, `tokenModifiers?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `tokenTypes` | `string`[] |
| `tokenModifiers?` | `string`[] |

#### Defined in

[index.d.ts:3731](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3731)

## Properties

### tokenModifiers

• `Readonly` **tokenModifiers**: `string`[]

The possible token modifiers.

#### Defined in

[index.d.ts:3729](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3729)

___

### tokenTypes

• `Readonly` **tokenTypes**: `string`[]

The possible token types.

#### Defined in

[index.d.ts:3725](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3725)
