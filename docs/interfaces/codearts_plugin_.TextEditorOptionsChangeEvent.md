[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditorOptionsChangeEvent

# Interface: TextEditorOptionsChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditorOptionsChangeEvent

Represents an event describing the change in a [text editor's options](codearts_plugin_.TextEditor.md#options).

## Table of contents

### Properties

- [options](codearts_plugin_.TextEditorOptionsChangeEvent.md#options)
- [textEditor](codearts_plugin_.TextEditorOptionsChangeEvent.md#texteditor)

## Properties

### options

• `Readonly` **options**: [`TextEditorOptions`](codearts_plugin_.TextEditorOptions.md)

The new value for the [text editor's options](codearts_plugin_.TextEditor.md#options).

#### Defined in

[index.d.ts:579](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L579)

___

### textEditor

• `Readonly` **textEditor**: [`TextEditor`](codearts_plugin_.TextEditor.md)

The [text editor](codearts_plugin_.TextEditor.md) for which the options have changed.

#### Defined in

[index.d.ts:575](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L575)
