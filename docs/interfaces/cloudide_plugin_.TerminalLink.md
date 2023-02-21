[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TerminalLink

# Interface: TerminalLink

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TerminalLink

A link on a terminal line.

## Table of contents

### Properties

- [length](cloudide_plugin_.TerminalLink.md#length)
- [startIndex](cloudide_plugin_.TerminalLink.md#startindex)
- [tooltip](cloudide_plugin_.TerminalLink.md#tooltip)

## Properties

### length

• **length**: `number`

The length of the link on [TerminalLinkContext.line](#TerminalLinkContext.line]

#### Defined in

[index.d.ts:2937](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2937)

___

### startIndex

• **startIndex**: `number`

The start index of the link on [TerminalLinkContext.line](#TerminalLinkContext.line].

#### Defined in

[index.d.ts:2932](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2932)

___

### tooltip

• `Optional` **tooltip**: `string`

The tooltip text when you hover over this link.

If a tooltip is provided, is will be displayed in a string that includes instructions on
how to trigger the link, such as `{0} (ctrl + click)`. The specific instructions vary
depending on OS, user settings, and localization.

#### Defined in

[index.d.ts:2946](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2946)
