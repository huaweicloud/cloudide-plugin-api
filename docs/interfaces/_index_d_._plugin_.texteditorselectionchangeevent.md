**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextEditorSelectionChangeEvent

# Interface: TextEditorSelectionChangeEvent

Represents an event describing the change in a [text editor's selections](#TextEditor.selections).

## Hierarchy

* **TextEditorSelectionChangeEvent**

## Index

### Properties

* [kind](_index_d_._plugin_.texteditorselectionchangeevent.md#kind)
* [selections](_index_d_._plugin_.texteditorselectionchangeevent.md#selections)
* [textEditor](_index_d_._plugin_.texteditorselectionchangeevent.md#texteditor)

## Properties

### kind

• `Optional` `Readonly` **kind**: [TextEditorSelectionChangeKind](../enums/_index_d_._plugin_.texteditorselectionchangekind.md)

*Defined in [index.d.ts:661](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L661)*

The [change kind](#TextEditorSelectionChangeKind) which has triggered this
event. Can be `undefined`.

___

### selections

• `Readonly` **selections**: ReadonlyArray\<[Selection](../classes/_index_d_._plugin_.selection.md)>

*Defined in [index.d.ts:656](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L656)*

The new value for the [text editor's selections](#TextEditor.selections).

___

### textEditor

• `Readonly` **textEditor**: [TextEditor](_index_d_._plugin_.texteditor.md)

*Defined in [index.d.ts:652](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L652)*

The [text editor](#TextEditor) for which the selections have changed.
