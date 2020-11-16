**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextEditorViewColumnChangeEvent

# Interface: TextEditorViewColumnChangeEvent

Represents an event describing the change of a [text editor's view column](#TextEditor.viewColumn).

## Hierarchy

* **TextEditorViewColumnChangeEvent**

## Index

### Properties

* [textEditor](_index_d_._plugin_.texteditorviewcolumnchangeevent.md#texteditor)
* [viewColumn](_index_d_._plugin_.texteditorviewcolumnchangeevent.md#viewcolumn)

## Properties

### textEditor

• `Readonly` **textEditor**: [TextEditor](_index_d_._plugin_.texteditor.md)

*Defined in [index.d.ts:589](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L589)*

The [text editor](#TextEditor) for which the view column has changed.

___

### viewColumn

• `Readonly` **viewColumn**: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md)

*Defined in [index.d.ts:593](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L593)*

The new value for the [text editor's view column](#TextEditor.viewColumn).
