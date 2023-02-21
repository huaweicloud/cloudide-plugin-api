[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextEditorSelectionChangeEvent

# Interface: TextEditorSelectionChangeEvent

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextEditorSelectionChangeEvent

Represents an event describing the change in text editor selections.

## Table of contents

### Properties

- [kind](cloudide_plugin_.TextEditorSelectionChangeEvent.md#kind)
- [selections](cloudide_plugin_.TextEditorSelectionChangeEvent.md#selections)
- [textEditor](cloudide_plugin_.TextEditorSelectionChangeEvent.md#texteditor)

## Properties

### kind

• `Optional` **kind**: [`TextEditorSelectionChangeKind`](../enums/cloudide_plugin_.TextEditorSelectionChangeKind.md)

#### Defined in

[index.d.ts:616](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L616)

___

### selections

• **selections**: [`Selection`](../classes/cloudide_plugin_.Selection.md)[]

The new text editor selections

#### Defined in

[index.d.ts:614](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L614)

___

### textEditor

• **textEditor**: [`TextEditor`](cloudide_plugin_.TextEditor.md)

The text editor for which the selections have changed.

#### Defined in

[index.d.ts:610](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L610)
