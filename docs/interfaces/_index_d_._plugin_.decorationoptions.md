**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DecorationOptions

# Interface: DecorationOptions

Represents options for a specific decoration in a [decoration set](#TextEditorDecorationType).

## Hierarchy

* **DecorationOptions**

## Index

### Properties

* [hoverMessage](_index_d_._plugin_.decorationoptions.md#hovermessage)
* [range](_index_d_._plugin_.decorationoptions.md#range)
* [renderOptions](_index_d_._plugin_.decorationoptions.md#renderoptions)

## Properties

### hoverMessage

• `Optional` **hoverMessage**: [MarkedString](../modules/_index_d_._plugin_.md#markedstring) \| [MarkedString](../modules/_index_d_._plugin_.md#markedstring)[]

*Defined in [index.d.ts:1054](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1054)*

A message that should be rendered when hovering over the decoration.

___

### range

•  **range**: [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:1049](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1049)*

Range to which this decoration is applied. The range must not be empty.

___

### renderOptions

• `Optional` **renderOptions**: [DecorationInstanceRenderOptions](_index_d_._plugin_.decorationinstancerenderoptions.md)

*Defined in [index.d.ts:1060](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1060)*

Render options applied to the current decoration. For performance reasons, keep the
number of decoration specific options small, and use decoration types wherever possible.
