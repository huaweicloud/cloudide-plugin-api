[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SignatureInformation

# Class: SignatureInformation

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SignatureInformation

Represents the signature of something callable. A signature
can have a label, like a function-name, a doc-comment, and
a set of parameters.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.SignatureInformation.md#constructor)

### Properties

- [documentation](cloudide_plugin_.SignatureInformation.md#documentation)
- [label](cloudide_plugin_.SignatureInformation.md#label)
- [parameters](cloudide_plugin_.SignatureInformation.md#parameters)

## Constructors

### constructor

• **new SignatureInformation**(`label`, `documentation?`)

Creates a new signature information object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` | A label string. |
| `documentation?` | `string` \| [`MarkdownString`](cloudide_plugin_.MarkdownString.md) | A doc string. |

#### Defined in

[index.d.ts:6782](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6782)

## Properties

### documentation

• `Optional` **documentation**: `string` \| [`MarkdownString`](cloudide_plugin_.MarkdownString.md)

The human-readable doc-comment of this signature. Will be shown
in the UI but can be omitted.

#### Defined in

[index.d.ts:6769](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6769)

___

### label

• **label**: `string`

The label of this signature. Will be shown in
the UI.

#### Defined in

[index.d.ts:6763](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6763)

___

### parameters

• **parameters**: [`ParameterInformation`](cloudide_plugin_.ParameterInformation.md)[]

The parameters of this signature.

#### Defined in

[index.d.ts:6774](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6774)
