[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SignatureInformation

# Class: SignatureInformation

["@codearts/plugin"](../modules/_codearts_plugin_.md).SignatureInformation

Represents the signature of something callable. A signature
can have a label, like a function-name, a doc-comment, and
a set of parameters.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SignatureInformation.md#constructor)

### Properties

- [activeParameter](codearts_plugin_.SignatureInformation.md#activeparameter)
- [documentation](codearts_plugin_.SignatureInformation.md#documentation)
- [label](codearts_plugin_.SignatureInformation.md#label)
- [parameters](codearts_plugin_.SignatureInformation.md#parameters)

## Constructors

### constructor

• **new SignatureInformation**(`label`, `documentation?`)

Creates a new signature information object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` | A label string. |
| `documentation?` | `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md) | A doc string. |

#### Defined in

[index.d.ts:4097](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4097)

## Properties

### activeParameter

• `Optional` **activeParameter**: `number`

The index of the active parameter.

If provided, this is used in place of [`activeSignature`](codearts_plugin_.SignatureHelp.md#activesignature).

#### Defined in

[index.d.ts:4089](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4089)

___

### documentation

• `Optional` **documentation**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

The human-readable doc-comment of this signature. Will be shown
in the UI but can be omitted.

#### Defined in

[index.d.ts:4077](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4077)

___

### label

• **label**: `string`

The label of this signature. Will be shown in
the UI.

#### Defined in

[index.d.ts:4071](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4071)

___

### parameters

• **parameters**: [`ParameterInformation`](codearts_plugin_.ParameterInformation.md)[]

The parameters of this signature.

#### Defined in

[index.d.ts:4082](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4082)
