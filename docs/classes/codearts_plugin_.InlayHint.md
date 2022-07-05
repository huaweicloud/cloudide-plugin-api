[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlayHint

# Class: InlayHint

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlayHint

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](codearts_plugin_.Position.md) |  |
| `label` | `string` \| [`InlayHintLabelPart`](codearts_plugin_.InlayHintLabelPart.md)[] |  |
| `kind?` | [`InlayHintKind`](../enums/codearts_plugin_.InlayHintKind.md) |  |

#### Defined in

[index.d.ts:4968](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L4968)

## Properties

### kind

• `Optional` **kind**: [`InlayHintKind`](../enums/codearts_plugin_.InlayHintKind.md)

#### Defined in

[index.d.ts:4933](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L4933)

___

### label

• **label**: `string` \| [`InlayHintLabelPart`](codearts_plugin_.InlayHintLabelPart.md)[]

#### Defined in

[index.d.ts:4920](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L4920)

___

### paddingLeft

• `Optional` **paddingLeft**: `boolean`

#### Defined in

[index.d.ts:4952](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L4952)

___

### paddingRight

• `Optional` **paddingRight**: `boolean`

#### Defined in

[index.d.ts:4959](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L4959)

___

### position

• **position**: [`Position`](codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:4913](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L4913)

___

### textEdits

• `Optional` **textEdits**: [`TextEdit`](codearts_plugin_.TextEdit.md)[]

#### Defined in

[index.d.ts:4945](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L4945)

___

### tooltip

• `Optional` **tooltip**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:4928](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L4928)
