[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditorSelectionChangeEvent

# Interface: TextEditorSelectionChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditorSelectionChangeEvent

Represents an event describing the change in a [text editor's selections](codearts_plugin_.TextEditor.md#selections).

## Table of contents

### Properties

- [kind](codearts_plugin_.TextEditorSelectionChangeEvent.md#kind)
- [selections](codearts_plugin_.TextEditorSelectionChangeEvent.md#selections)
- [textEditor](codearts_plugin_.TextEditorSelectionChangeEvent.md#texteditor)

## Properties

### kind

• `Readonly` **kind**: `undefined` \| [`TextEditorSelectionChangeKind`](../enums/codearts_plugin_.TextEditorSelectionChangeKind.md)

The [change kind](../enums/codearts_plugin_.TextEditorSelectionChangeKind.md) which has triggered this
event. Can be `undefined`.

#### Defined in

[index.d.ts:551](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L551)

___

### selections

• `Readonly` **selections**: readonly [`Selection`](../classes/codearts_plugin_.Selection.md)[]

The new value for the [text editor's selections](codearts_plugin_.TextEditor.md#selections).

#### Defined in

[index.d.ts:546](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L546)

___

### textEditor

• `Readonly` **textEditor**: [`TextEditor`](codearts_plugin_.TextEditor.md)

The [text editor](codearts_plugin_.TextEditor.md) for which the selections have changed.

#### Defined in

[index.d.ts:542](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L542)
