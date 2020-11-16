**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextEditorVisibleRangesChangeEvent

# Interface: TextEditorVisibleRangesChangeEvent

Represents an event describing the change in a [text editor's visible ranges](#TextEditor.visibleRanges).

## Hierarchy

* **TextEditorVisibleRangesChangeEvent**

## Index

### Properties

* [textEditor](_index_d_._plugin_.texteditorvisiblerangeschangeevent.md#texteditor)
* [visibleRanges](_index_d_._plugin_.texteditorvisiblerangeschangeevent.md#visibleranges)

## Properties

### textEditor

• `Readonly` **textEditor**: [TextEditor](_index_d_._plugin_.texteditor.md)

*Defined in [index.d.ts:561](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L561)*

The [text editor](#TextEditor) for which the visible ranges have changed.

___

### visibleRanges

• `Readonly` **visibleRanges**: ReadonlyArray\<[Range](../classes/_index_d_._plugin_.range.md)>

*Defined in [index.d.ts:565](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L565)*

The new value for the [text editor's visible ranges](#TextEditor.visibleRanges).
