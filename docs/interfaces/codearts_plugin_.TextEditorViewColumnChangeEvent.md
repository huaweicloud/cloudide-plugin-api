[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditorViewColumnChangeEvent

# Interface: TextEditorViewColumnChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditorViewColumnChangeEvent

Represents an event describing the change of a [text editor's view column](codearts_plugin_.TextEditor.md#viewcolumn).

## Table of contents

### Properties

- [textEditor](codearts_plugin_.TextEditorViewColumnChangeEvent.md#texteditor)
- [viewColumn](codearts_plugin_.TextEditorViewColumnChangeEvent.md#viewcolumn)

## Properties

### textEditor

• `Readonly` **textEditor**: [`TextEditor`](codearts_plugin_.TextEditor.md)

The [text editor](codearts_plugin_.TextEditor.md) for which the view column has changed.

#### Defined in

[index.d.ts:589](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L589)

___

### viewColumn

• `Readonly` **viewColumn**: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)

The new value for the [text editor's view column](codearts_plugin_.TextEditor.md#viewcolumn).

#### Defined in

[index.d.ts:593](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L593)
