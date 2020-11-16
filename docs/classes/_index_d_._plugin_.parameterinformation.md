**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ParameterInformation

# Class: ParameterInformation

Represents a parameter of a callable-signature. A parameter can
have a label and a doc-comment.

## Hierarchy

* **ParameterInformation**

## Index

### Constructors

* [constructor](_index_d_._plugin_.parameterinformation.md#constructor)

### Properties

* [documentation](_index_d_._plugin_.parameterinformation.md#documentation)
* [label](_index_d_._plugin_.parameterinformation.md#label)

## Constructors

### constructor

\+ **new ParameterInformation**(`label`: string \| [number, number], `documentation?`: string \| [MarkdownString](_index_d_._plugin_.markdownstring.md)): [ParameterInformation](_index_d_._plugin_.parameterinformation.md)

*Defined in [index.d.ts:3515](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3515)*

Creates a new parameter information object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`label` | string \| [number, number] | A label string or inclusive start and exclusive end offsets within its containing signature label. |
`documentation?` | string \| [MarkdownString](_index_d_._plugin_.markdownstring.md) | A doc string.  |

**Returns:** [ParameterInformation](_index_d_._plugin_.parameterinformation.md)

## Properties

### documentation

• `Optional` **documentation**: string \| [MarkdownString](_index_d_._plugin_.markdownstring.md)

*Defined in [index.d.ts:3515](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3515)*

The human-readable doc-comment of this signature. Will be shown
in the UI but can be omitted.

___

### label

•  **label**: string \| [number, number]

*Defined in [index.d.ts:3509](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3509)*

The label of this signature.

Either a string or inclusive start and exclusive end offsets within its containing
[signature label](#SignatureInformation.label). *Note*: A label of type string must be
a substring of its containing signature information's [label](#SignatureInformation.label).
