[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DecorationOptions

# Interface: DecorationOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).DecorationOptions

Represents options for a specific decoration in a [decoration set](codearts_plugin_.TextEditorDecorationType.md).

## Table of contents

### Properties

- [hoverMessage](codearts_plugin_.DecorationOptions.md#hovermessage)
- [range](codearts_plugin_.DecorationOptions.md#range)
- [renderOptions](codearts_plugin_.DecorationOptions.md#renderoptions)

## Properties

### hoverMessage

• `Optional` **hoverMessage**: [`MarkdownString`](../classes/codearts_plugin_.MarkdownString.md) \| [`MarkedString`](../modules/_codearts_plugin_.md#markedstring) \| ([`MarkdownString`](../classes/codearts_plugin_.MarkdownString.md) \| [`MarkedString`](../modules/_codearts_plugin_.md#markedstring))[]

A message that should be rendered when hovering over the decoration.

#### Defined in

[index.d.ts:1128](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1128)

___

### range

• **range**: [`Range`](../classes/codearts_plugin_.Range.md)

Range to which this decoration is applied. The range must not be empty.

#### Defined in

[index.d.ts:1123](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1123)

___

### renderOptions

• `Optional` **renderOptions**: [`DecorationInstanceRenderOptions`](codearts_plugin_.DecorationInstanceRenderOptions.md)

Render options applied to the current decoration. For performance reasons, keep the
number of decoration specific options small, and use decoration types wherever possible.

#### Defined in

[index.d.ts:1134](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1134)
