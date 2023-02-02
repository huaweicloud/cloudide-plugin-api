[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ParameterInformation

# Class: ParameterInformation

["@codearts/plugin"](../modules/_codearts_plugin_.md).ParameterInformation

Represents a parameter of a callable-signature. A parameter can
have a label and a doc-comment.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.ParameterInformation.md#constructor)

### Properties

- [documentation](codearts_plugin_.ParameterInformation.md#documentation)
- [label](codearts_plugin_.ParameterInformation.md#label)

## Constructors

### constructor

• **new ParameterInformation**(`label`, `documentation?`)

Creates a new parameter information object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` \| [`number`, `number`] | A label string or inclusive start and exclusive end offsets within its containing signature label. |
| `documentation?` | `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md) | A doc string. |

#### Defined in

[index.d.ts:4019](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4019)

## Properties

### documentation

• `Optional` **documentation**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

The human-readable doc-comment of this signature. Will be shown
in the UI but can be omitted.

#### Defined in

[index.d.ts:4011](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4011)

___

### label

• **label**: `string` \| [`number`, `number`]

The label of this signature.

Either a string or inclusive start and exclusive end offsets within its containing
[signature label](codearts_plugin_.SignatureInformation.md#label). *Note*: A label of type string must be
a substring of its containing signature information's [label](codearts_plugin_.SignatureInformation.md#label).

#### Defined in

[index.d.ts:4005](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4005)
