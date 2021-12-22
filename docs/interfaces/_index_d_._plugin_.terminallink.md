**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TerminalLink

# Interface: TerminalLink

A link on a terminal line.

## Hierarchy

* **TerminalLink**

## Index

### Properties

* [length](_index_d_._plugin_.terminallink.md#length)
* [startIndex](_index_d_._plugin_.terminallink.md#startindex)
* [tooltip](_index_d_._plugin_.terminallink.md#tooltip)

## Properties

### length

•  **length**: number

*Defined in [index.d.ts:5732](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5732)*

The length of the link on [TerminalLinkContext.line](#TerminalLinkContext.line]

___

### startIndex

•  **startIndex**: number

*Defined in [index.d.ts:5727](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5727)*

The start index of the link on [TerminalLinkContext.line](#TerminalLinkContext.line].

___

### tooltip

• `Optional` **tooltip**: string

*Defined in [index.d.ts:5741](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5741)*

The tooltip text when you hover over this link.

If a tooltip is provided, is will be displayed in a string that includes instructions on
how to trigger the link, such as `{0} (ctrl + click)`. The specific instructions vary
depending on OS, user settings, and localization.
