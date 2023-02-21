[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DecorationOptions

# Interface: DecorationOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DecorationOptions

Represents options for a specific decoration in a [decoration set](#TextEditorDecorationType).

## Table of contents

### Properties

- [hoverMessage](cloudide_plugin_.DecorationOptions.md#hovermessage)
- [range](cloudide_plugin_.DecorationOptions.md#range)
- [renderOptions](cloudide_plugin_.DecorationOptions.md#renderoptions)

## Properties

### hoverMessage

• `Optional` **hoverMessage**: [`MarkedString`](../modules/_cloudide_plugin_.md#markedstring) \| [`MarkedString`](../modules/_cloudide_plugin_.md#markedstring)[]

A message that should be rendered when hovering over the decoration.

#### Defined in

[index.d.ts:932](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L932)

___

### range

• **range**: [`Range`](../classes/cloudide_plugin_.Range.md)

Range to which this decoration is applied. The range must not be empty.

#### Defined in

[index.d.ts:927](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L927)

___

### renderOptions

• `Optional` **renderOptions**: [`DecorationInstanceRenderOptions`](cloudide_plugin_.DecorationInstanceRenderOptions.md)

Render options applied to the current decoration. For performance reasons, keep the
number of decoration specific options small, and use decoration types wherever possible.

#### Defined in

[index.d.ts:938](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L938)
