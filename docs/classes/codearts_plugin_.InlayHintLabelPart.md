[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlayHintLabelPart

# Class: InlayHintLabelPart

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlayHintLabelPart

An inlay hint label part allows for interactive and composite labels of inlay hints.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.InlayHintLabelPart.md#constructor)

### Properties

- [command](codearts_plugin_.InlayHintLabelPart.md#command)
- [location](codearts_plugin_.InlayHintLabelPart.md#location)
- [tooltip](codearts_plugin_.InlayHintLabelPart.md#tooltip)
- [value](codearts_plugin_.InlayHintLabelPart.md#value)

## Constructors

### constructor

• **new InlayHintLabelPart**(`value`)

Creates a new inlay hint label part.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | The value of the part. |

#### Defined in

[index.d.ts:4973](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4973)

## Properties

### command

• `Optional` **command**: [`Command`](../interfaces/codearts_plugin_.Command.md)

An optional command for this label part.

The editor renders parts with commands as clickable links. The command is added to the context menu
when a label part defines [location](codearts_plugin_.InlayHintLabelPart.md#location) and [command](codearts_plugin_.InlayHintLabelPart.md#command) .

*Note* that this property can be set late during
[resolving](../interfaces/codearts_plugin_.InlayHintsProvider.md#resolveinlayhint) of inlay hints.

#### Defined in

[index.d.ts:4966](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4966)

___

### location

• `Optional` **location**: [`Location`](codearts_plugin_.Location.md)

An optional [source code location](codearts_plugin_.Location.md) that represents this label
part.

The editor will use this location for the hover and for code navigation features: This
part will become a clickable link that resolves to the definition of the symbol at the
given location (not necessarily the location itself), it shows the hover that shows at
the given location, and it shows a context menu with further code navigation commands.

*Note* that this property can be set late during
[resolving](../interfaces/codearts_plugin_.InlayHintsProvider.md#resolveinlayhint) of inlay hints.

#### Defined in

[index.d.ts:4955](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4955)

___

### tooltip

• `Optional` **tooltip**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

The tooltip text when you hover over this label part.

*Note* that this property can be set late during
[resolving](../interfaces/codearts_plugin_.InlayHintsProvider.md#resolveinlayhint) of inlay hints.

#### Defined in

[index.d.ts:4941](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4941)

___

### value

• **value**: `string`

The value of this label part.

#### Defined in

[index.d.ts:4933](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4933)
