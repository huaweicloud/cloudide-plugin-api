[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextEditorOptions

# Interface: TextEditorOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextEditorOptions

Represents a text editor's options

## Table of contents

### Properties

- [cursorStyle](cloudide_plugin_.TextEditorOptions.md#cursorstyle)
- [insertSpaces](cloudide_plugin_.TextEditorOptions.md#insertspaces)
- [lineNumbers](cloudide_plugin_.TextEditorOptions.md#linenumbers)
- [tabSize](cloudide_plugin_.TextEditorOptions.md#tabsize)

## Properties

### cursorStyle

• `Optional` **cursorStyle**: [`TextEditorCursorStyle`](../enums/cloudide_plugin_.TextEditorCursorStyle.md)

The rendering style of the cursor in this editor.
When getting a text editor's options, this property will always be present.
When setting a text editor's options, this property is optional.

#### Defined in

[index.d.ts:1948](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1948)

___

### insertSpaces

• `Optional` **insertSpaces**: `string` \| `boolean`

When pressing Tab insert [n](#TextEditorOptions.tabSize) spaces.
When getting a text editor's options, this property will always be a boolean (resolved).
When setting a text editor's options, this property is optional and it can be a boolean or `"auto"`.

#### Defined in

[index.d.ts:1941](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1941)

___

### lineNumbers

• `Optional` **lineNumbers**: [`TextEditorLineNumbersStyle`](../enums/cloudide_plugin_.TextEditorLineNumbersStyle.md)

Render relative line numbers w.r.t. the current line number.
When getting a text editor's options, this property will always be present.
When setting a text editor's options, this property is optional.

#### Defined in

[index.d.ts:1955](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1955)

___

### tabSize

• `Optional` **tabSize**: `string` \| `number`

The size in spaces a tab takes. This is used for two purposes:
 - the rendering width of a tab character;
 - the number of spaces to insert when [insertSpaces](#TextEditorOptions.insertSpaces) is true.

When getting a text editor's options, this property will always be a number (resolved).
When setting a text editor's options, this property is optional and it can be a number or `"auto"`.

#### Defined in

[index.d.ts:1934](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1934)
