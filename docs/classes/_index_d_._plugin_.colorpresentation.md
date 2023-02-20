**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ColorPresentation

# Class: ColorPresentation

A color presentation object describes how a [`color`](#Color) should be represented as text and what
edits are required to refer to it from source code.

For some languages one color can have multiple presentations, e.g. css can represent the color red with
the constant `Red`, the hex-value `#ff0000`, or in rgba and hsla forms. In csharp other representations
apply, e.g. `System.Drawing.Color.Red`.

## Hierarchy

* **ColorPresentation**

## Index

### Constructors

* [constructor](_index_d_._plugin_.colorpresentation.md#constructor)

### Properties

* [additionalTextEdits](_index_d_._plugin_.colorpresentation.md#additionaltextedits)
* [label](_index_d_._plugin_.colorpresentation.md#label)
* [textEdit](_index_d_._plugin_.colorpresentation.md#textedit)

## Constructors

### constructor

\+ **new ColorPresentation**(`label`: string): [ColorPresentation](_index_d_._plugin_.colorpresentation.md)

*Defined in [index.d.ts:4371](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4371)*

Creates a new color presentation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`label` | string | The label of this color presentation.  |

**Returns:** [ColorPresentation](_index_d_._plugin_.colorpresentation.md)

## Properties

### additionalTextEdits

• `Optional` **additionalTextEdits**: [TextEdit](_index_d_._plugin_.textedit.md)[]

*Defined in [index.d.ts:4371](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4371)*

An optional array of additional [text edits](#TextEdit) that are applied when
selecting this color presentation. Edits must not overlap with the main [edit](#ColorPresentation.textEdit) nor with themselves.

___

### label

•  **label**: string

*Defined in [index.d.ts:4358](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4358)*

The label of this color presentation. It will be shown on the color
picker header. By default this is also the text that is inserted when selecting
this color presentation.

___

### textEdit

• `Optional` **textEdit**: [TextEdit](_index_d_._plugin_.textedit.md)

*Defined in [index.d.ts:4365](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4365)*

An [edit](#TextEdit) which is applied to a document when selecting
this presentation for the color.  When `falsy` the [label](#ColorPresentation.label)
is used.
