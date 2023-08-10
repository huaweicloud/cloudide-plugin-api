[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlayHint

# Class: InlayHint

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlayHint

Inlay hint information.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.InlayHint.md#constructor)

### Properties

- [kind](codearts_plugin_.InlayHint.md#kind)
- [label](codearts_plugin_.InlayHint.md#label)
- [paddingLeft](codearts_plugin_.InlayHint.md#paddingleft)
- [paddingRight](codearts_plugin_.InlayHint.md#paddingright)
- [position](codearts_plugin_.InlayHint.md#position)
- [textEdits](codearts_plugin_.InlayHint.md#textedits)
- [tooltip](codearts_plugin_.InlayHint.md#tooltip)

## Constructors

### constructor

• **new InlayHint**(`position`, `label`, `kind?`)

Creates a new inlay hint.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](codearts_plugin_.Position.md) | The position of the hint. |
| `label` | `string` \| [`InlayHintLabelPart`](codearts_plugin_.InlayHintLabelPart.md)[] | The label of the hint. |
| `kind?` | [`InlayHintKind`](../enums/codearts_plugin_.InlayHintKind.md) | The [kind](../enums/codearts_plugin_.InlayHintKind.md) of the hint. |

#### Defined in

[index.d.ts:5039](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5039)

## Properties

### kind

• `Optional` **kind**: [`InlayHintKind`](../enums/codearts_plugin_.InlayHintKind.md)

The kind of this hint. The inlay hint kind defines the appearance of this inlay hint.

#### Defined in

[index.d.ts:5004](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5004)

___

### label

• **label**: `string` \| [`InlayHintLabelPart`](codearts_plugin_.InlayHintLabelPart.md)[]

The label of this hint. A human readable string or an array of [label parts](codearts_plugin_.InlayHintLabelPart.md).

*Note* that neither the string nor the label part can be empty.

#### Defined in

[index.d.ts:4991](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4991)

___

### paddingLeft

• `Optional` **paddingLeft**: `boolean`

Render padding before the hint. Padding will use the editor's background color,
not the background color of the hint itself. That means padding can be used to visually
align/separate an inlay hint.

#### Defined in

[index.d.ts:5023](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5023)

___

### paddingRight

• `Optional` **paddingRight**: `boolean`

Render padding after the hint. Padding will use the editor's background color,
not the background color of the hint itself. That means padding can be used to visually
align/separate an inlay hint.

#### Defined in

[index.d.ts:5030](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5030)

___

### position

• **position**: [`Position`](codearts_plugin_.Position.md)

The position of this hint.

#### Defined in

[index.d.ts:4984](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4984)

___

### textEdits

• `Optional` **textEdits**: [`TextEdit`](codearts_plugin_.TextEdit.md)[]

Optional [text edits](codearts_plugin_.TextEdit.md) that are performed when accepting this inlay hint. The default
gesture for accepting an inlay hint is the double click.

*Note* that edits are expected to change the document so that the inlay hint (or its nearest variant) is
now part of the document and the inlay hint itself is now obsolete.

*Note* that this property can be set late during
[resolving](../interfaces/codearts_plugin_.InlayHintsProvider.md#resolveinlayhint) of inlay hints.

#### Defined in

[index.d.ts:5016](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5016)

___

### tooltip

• `Optional` **tooltip**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

The tooltip text when you hover over this item.

*Note* that this property can be set late during
[resolving](../interfaces/codearts_plugin_.InlayHintsProvider.md#resolveinlayhint) of inlay hints.

#### Defined in

[index.d.ts:4999](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4999)
