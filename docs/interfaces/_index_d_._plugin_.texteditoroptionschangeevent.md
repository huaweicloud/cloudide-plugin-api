**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextEditorOptionsChangeEvent

# Interface: TextEditorOptionsChangeEvent

Represents an event describing the change in a [text editor's options](#TextEditor.options).

## Hierarchy

* **TextEditorOptionsChangeEvent**

## Index

### Properties

* [options](_index_d_._plugin_.texteditoroptionschangeevent.md#options)
* [textEditor](_index_d_._plugin_.texteditoroptionschangeevent.md#texteditor)

## Properties

### options

• `Readonly` **options**: [TextEditorOptions](_index_d_._plugin_.texteditoroptions.md)

*Defined in [index.d.ts:692](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L692)*

The new value for the [text editor's options](#TextEditor.options).

___

### textEditor

• `Readonly` **textEditor**: [TextEditor](_index_d_._plugin_.texteditor.md)

*Defined in [index.d.ts:688](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L688)*

The [text editor](#TextEditor) for which the options have changed.
