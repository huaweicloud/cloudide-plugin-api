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

*Defined in [index.d.ts:1175](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1175)*

A message that should be rendered when hovering over the decoration.

___

### range

•  **range**: [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:1170](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1170)*

Range to which this decoration is applied. The range must not be empty.

___

### renderOptions

• `Optional` **renderOptions**: [DecorationInstanceRenderOptions](_index_d_._plugin_.decorationinstancerenderoptions.md)

*Defined in [index.d.ts:1181](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1181)*

Render options applied to the current decoration. For performance reasons, keep the
number of decoration specific options small, and use decoration types wherever possible.
