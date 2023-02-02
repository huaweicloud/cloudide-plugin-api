[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ColorPresentation

# Class: ColorPresentation

["@codearts/plugin"](../modules/_codearts_plugin_.md).ColorPresentation

A color presentation object describes how a [`Color`](codearts_plugin_.Color.md) should be represented as text and what
edits are required to refer to it from source code.

For some languages one color can have multiple presentations, e.g. css can represent the color red with
the constant `Red`, the hex-value `#ff0000`, or in rgba and hsla forms. In csharp other representations
apply, e.g. `System.Drawing.Color.Red`.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.ColorPresentation.md#constructor)

### Properties

- [additionalTextEdits](codearts_plugin_.ColorPresentation.md#additionaltextedits)
- [label](codearts_plugin_.ColorPresentation.md#label)
- [textEdit](codearts_plugin_.ColorPresentation.md#textedit)

## Constructors

### constructor

• **new ColorPresentation**(`label`)

Creates a new color presentation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` | The label of this color presentation. |

#### Defined in

[index.d.ts:4826](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4826)

## Properties

### additionalTextEdits

• `Optional` **additionalTextEdits**: [`TextEdit`](codearts_plugin_.TextEdit.md)[]

An optional array of additional [text edits](codearts_plugin_.TextEdit.md) that are applied when
selecting this color presentation. Edits must not overlap with the main [edit](codearts_plugin_.ColorPresentation.md#textedit) nor with themselves.

#### Defined in

[index.d.ts:4819](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4819)

___

### label

• **label**: `string`

The label of this color presentation. It will be shown on the color
picker header. By default this is also the text that is inserted when selecting
this color presentation.

#### Defined in

[index.d.ts:4806](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4806)

___

### textEdit

• `Optional` **textEdit**: [`TextEdit`](codearts_plugin_.TextEdit.md)

An [edit](codearts_plugin_.TextEdit.md) which is applied to a document when selecting
this presentation for the color.  When `falsy` the [label](codearts_plugin_.ColorPresentation.md#label)
is used.

#### Defined in

[index.d.ts:4813](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4813)
