[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditorVisibleRangesChangeEvent

# Interface: TextEditorVisibleRangesChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditorVisibleRangesChangeEvent

Represents an event describing the change in a [text editor's visible ranges](codearts_plugin_.TextEditor.md#visibleranges).

## Table of contents

### Properties

- [textEditor](codearts_plugin_.TextEditorVisibleRangesChangeEvent.md#texteditor)
- [visibleRanges](codearts_plugin_.TextEditorVisibleRangesChangeEvent.md#visibleranges)

## Properties

### textEditor

• `Readonly` **textEditor**: [`TextEditor`](codearts_plugin_.TextEditor.md)

The [text editor](codearts_plugin_.TextEditor.md) for which the visible ranges have changed.

#### Defined in

[index.d.ts:561](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L561)

___

### visibleRanges

• `Readonly` **visibleRanges**: readonly [`Range`](../classes/codearts_plugin_.Range.md)[]

The new value for the [text editor's visible ranges](codearts_plugin_.TextEditor.md#visibleranges).

#### Defined in

[index.d.ts:565](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L565)
