**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextEditorOptions

# Interface: TextEditorOptions

Represents a [text editor](#TextEditor)'s [options](#TextEditor.options).

## Hierarchy

* **TextEditorOptions**

## Index

### Properties

* [cursorStyle](_index_d_._plugin_.texteditoroptions.md#cursorstyle)
* [insertSpaces](_index_d_._plugin_.texteditoroptions.md#insertspaces)
* [lineNumbers](_index_d_._plugin_.texteditoroptions.md#linenumbers)
* [tabSize](_index_d_._plugin_.texteditoroptions.md#tabsize)

## Properties

### cursorStyle

• `Optional` **cursorStyle**: [TextEditorCursorStyle](../enums/_index_d_._plugin_.texteditorcursorstyle.md)

*Defined in [index.d.ts:781](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L781)*

The rendering style of the cursor in this editor.
When getting a text editor's options, this property will always be present.
When setting a text editor's options, this property is optional.

___

### insertSpaces

• `Optional` **insertSpaces**: boolean \| string

*Defined in [index.d.ts:774](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L774)*

When pressing Tab insert [n](#TextEditorOptions.tabSize) spaces.
When getting a text editor's options, this property will always be a boolean (resolved).
When setting a text editor's options, this property is optional and it can be a boolean or `"auto"`.

___

### lineNumbers

• `Optional` **lineNumbers**: [TextEditorLineNumbersStyle](../enums/_index_d_._plugin_.texteditorlinenumbersstyle.md)

*Defined in [index.d.ts:788](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L788)*

Render relative line numbers w.r.t. the current line number.
When getting a text editor's options, this property will always be present.
When setting a text editor's options, this property is optional.

___

### tabSize

• `Optional` **tabSize**: number \| string

*Defined in [index.d.ts:767](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L767)*

The size in spaces a tab takes. This is used for two purposes:
 - the rendering width of a tab character;
 - the number of spaces to insert when [insertSpaces](#TextEditorOptions.insertSpaces) is true.

When getting a text editor's options, this property will always be a number (resolved).
When setting a text editor's options, this property is optional and it can be a number or `"auto"`.
