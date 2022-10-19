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

[index.d.ts:4059](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L4059)

## Properties

### activeParameter

• `Optional` **activeParameter**: `number`

The index of the active parameter.

If provided, this is used in place of [`activeSignature`](codearts_plugin_.SignatureHelp.md#activesignature).

#### Defined in

[index.d.ts:4051](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L4051)

___

### documentation

• `Optional` **documentation**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

The human-readable doc-comment of this signature. Will be shown
in the UI but can be omitted.

#### Defined in

[index.d.ts:4039](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L4039)

___

### label

• **label**: `string`

The label of this signature. Will be shown in
the UI.

#### Defined in

[index.d.ts:4033](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L4033)

___

### parameters

• **parameters**: [`ParameterInformation`](codearts_plugin_.ParameterInformation.md)[]

The parameters of this signature.

#### Defined in

[index.d.ts:4044](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L4044)
