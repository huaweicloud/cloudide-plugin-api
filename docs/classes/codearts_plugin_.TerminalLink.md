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

[index.d.ts:6740](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6740)

## Properties

### length

• **length**: `number`

The length of the link on [line](../interfaces/codearts_plugin_.TerminalLinkContext.md#line).

#### Defined in

[index.d.ts:6719](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6719)

___

### startIndex

• **startIndex**: `number`

The start index of the link on [line](../interfaces/codearts_plugin_.TerminalLinkContext.md#line).

#### Defined in

[index.d.ts:6714](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6714)

___

### tooltip

• `Optional` **tooltip**: `string`

The tooltip text when you hover over this link.

If a tooltip is provided, is will be displayed in a string that includes instructions on
how to trigger the link, such as `{0} (ctrl + click)`. The specific instructions vary
depending on OS, user settings, and localization.

#### Defined in

[index.d.ts:6728](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6728)
