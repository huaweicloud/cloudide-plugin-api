[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditorOptions

# Interface: TextEditorOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditorOptions

Represents a [text editor](codearts_plugin_.TextEditor.md)'s [options](codearts_plugin_.TextEditor.md#options).

## Table of contents

### Properties

- [cursorStyle](codearts_plugin_.TextEditorOptions.md#cursorstyle)
- [insertSpaces](codearts_plugin_.TextEditorOptions.md#insertspaces)
- [lineNumbers](codearts_plugin_.TextEditorOptions.md#linenumbers)
- [tabSize](codearts_plugin_.TextEditorOptions.md#tabsize)

## Properties

### cursorStyle

• `Optional` **cursorStyle**: [`TextEditorCursorStyle`](../enums/codearts_plugin_.TextEditorCursorStyle.md)

The rendering style of the cursor in this editor.
When getting a text editor's options, this property will always be present.
When setting a text editor's options, this property is optional.

#### Defined in

[index.d.ts:671](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L671)

___

### insertSpaces

• `Optional` **insertSpaces**: `string` \| `boolean`

When pressing Tab insert [n](codearts_plugin_.TextEditorOptions.md#tabsize) spaces.
When getting a text editor's options, this property will always be a boolean (resolved).
When setting a text editor's options, this property is optional and it can be a boolean or `"auto"`.

#### Defined in

[index.d.ts:664](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L664)

___

### lineNumbers

• `Optional` **lineNumbers**: [`TextEditorLineNumbersStyle`](../enums/codearts_plugin_.TextEditorLineNumbersStyle.md)

Render relative line numbers w.r.t. the current line number.
When getting a text editor's options, this property will always be present.
When setting a text editor's options, this property is optional.

#### Defined in

[index.d.ts:678](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L678)

___

### tabSize

• `Optional` **tabSize**: `string` \| `number`

The size in spaces a tab takes. This is used for two purposes:
 - the rendering width of a tab character;
 - the number of spaces to insert when [insertSpaces](codearts_plugin_.TextEditorOptions.md#insertspaces) is true.

When getting a text editor's options, this property will always be a number (resolved).
When setting a text editor's options, this property is optional and it can be a number or `"auto"`.

#### Defined in

[index.d.ts:657](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L657)
