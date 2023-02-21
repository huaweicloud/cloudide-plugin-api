[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ColorPresentation

# Class: ColorPresentation

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ColorPresentation

A color presentation object describes how a [`color`](#Color) should be represented as text and what
edits are required to refer to it from source code.

For some languages one color can have multiple presentations, e.g. css can represent the color red with
the constant `Red`, the hex-value `#ff0000`, or in rgba and hsla forms. In csharp other representations
apply, e.g `System.Drawing.Color.Red`.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.ColorPresentation.md#constructor)

### Properties

- [additionalTextEdits](cloudide_plugin_.ColorPresentation.md#additionaltextedits)
- [label](cloudide_plugin_.ColorPresentation.md#label)
- [textEdit](cloudide_plugin_.ColorPresentation.md#textedit)

## Constructors

### constructor

• **new ColorPresentation**(`label`)

Creates a new color presentation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` | The label of this color presentation. |

#### Defined in

[index.d.ts:7200](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7200)

## Properties

### additionalTextEdits

• `Optional` **additionalTextEdits**: [`TextEdit`](cloudide_plugin_.TextEdit.md)[]

An optional array of additional [text edits](#TextEdit) that are applied when
selecting this color presentation. Edits must not overlap with the main [edit](#ColorPresentation.textEdit) nor with themselves.

#### Defined in

[index.d.ts:7193](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7193)

___

### label

• **label**: `string`

The label of this color presentation. It will be shown on the color
picker header. By default this is also the text that is inserted when selecting
this color presentation.

#### Defined in

[index.d.ts:7180](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7180)

___

### textEdit

• `Optional` **textEdit**: [`TextEdit`](cloudide_plugin_.TextEdit.md)

An [edit](#TextEdit) which is applied to a document when selecting
this presentation for the color.  When `falsy` the [label](#ColorPresentation.label)
is used.

#### Defined in

[index.d.ts:7187](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7187)
