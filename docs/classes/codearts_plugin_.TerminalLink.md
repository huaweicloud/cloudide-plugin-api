[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TerminalLink

# Class: TerminalLink

["@codearts/plugin"](../modules/_codearts_plugin_.md).TerminalLink

A link on a terminal line.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TerminalLink.md#constructor)

### Properties

- [length](codearts_plugin_.TerminalLink.md#length)
- [startIndex](codearts_plugin_.TerminalLink.md#startindex)
- [tooltip](codearts_plugin_.TerminalLink.md#tooltip)

## Constructors

### constructor

• **new TerminalLink**(`startIndex`, `length`, `tooltip?`)

Creates a new terminal link.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startIndex` | `number` | The start index of the link on [line](../interfaces/codearts_plugin_.TerminalLinkContext.md#line). |
| `length` | `number` | The length of the link on [line](../interfaces/codearts_plugin_.TerminalLinkContext.md#line). |
| `tooltip?` | `string` | The tooltip text when you hover over this link.  If a tooltip is provided, is will be displayed in a string that includes instructions on how to trigger the link, such as `{0} (ctrl + click)`. The specific instructions vary depending on OS, user settings, and localization. |

#### Defined in

[index.d.ts:6711](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6711)

## Properties

### length

• **length**: `number`

The length of the link on [line](../interfaces/codearts_plugin_.TerminalLinkContext.md#line).

#### Defined in

[index.d.ts:6690](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6690)

___

### startIndex

• **startIndex**: `number`

The start index of the link on [line](../interfaces/codearts_plugin_.TerminalLinkContext.md#line).

#### Defined in

[index.d.ts:6685](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6685)

___

### tooltip

• `Optional` **tooltip**: `string`

The tooltip text when you hover over this link.

If a tooltip is provided, is will be displayed in a string that includes instructions on
how to trigger the link, such as `{0} (ctrl + click)`. The specific instructions vary
depending on OS, user settings, and localization.

#### Defined in

[index.d.ts:6699](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6699)
