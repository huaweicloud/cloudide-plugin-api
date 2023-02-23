[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ParameterInformation

# Class: ParameterInformation

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ParameterInformation

Represents a parameter of a callable-signature. A parameter can
have a label and a doc-comment.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.ParameterInformation.md#constructor)

### Properties

- [documentation](cloudide_plugin_.ParameterInformation.md#documentation)
- [label](cloudide_plugin_.ParameterInformation.md#label)

## Constructors

### constructor

• **new ParameterInformation**(`label`, `documentation?`)

Creates a new parameter information object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` \| [`number`, `number`] | A label string or inclusive start and exclusive end offsets within its containing signature label. |
| `documentation?` | `string` \| [`MarkdownString`](cloudide_plugin_.MarkdownString.md) | A doc string. |

#### Defined in

[index.d.ts:6748](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6748)

## Properties

### documentation

• `Optional` **documentation**: `string` \| [`MarkdownString`](cloudide_plugin_.MarkdownString.md)

The human-readable doc-comment of this signature. Will be shown
in the UI but can be omitted.

#### Defined in

[index.d.ts:6740](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6740)

___

### label

• **label**: `string` \| [`number`, `number`]

The label of this signature. Will be shown in
the UI.

#### Defined in

[index.d.ts:6734](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6734)
