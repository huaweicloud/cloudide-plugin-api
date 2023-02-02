[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookEditorSelectionChangeEvent

# Interface: NotebookEditorSelectionChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookEditorSelectionChangeEvent

Represents an event describing the change in a [notebook editor's selections](codearts_plugin_.NotebookEditor.md#selections).

## Table of contents

### Properties

- [notebookEditor](codearts_plugin_.NotebookEditorSelectionChangeEvent.md#notebookeditor)
- [selections](codearts_plugin_.NotebookEditorSelectionChangeEvent.md#selections)

## Properties

### notebookEditor

• `Readonly` **notebookEditor**: [`NotebookEditor`](codearts_plugin_.NotebookEditor.md)

The [notebook editor](codearts_plugin_.NotebookEditor.md) for which the selections have changed.

#### Defined in

[index.d.ts:796](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L796)

___

### selections

• `Readonly` **selections**: readonly [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md)[]

The new value for the [notebook editor's selections](codearts_plugin_.NotebookEditor.md#selections).

#### Defined in

[index.d.ts:801](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L801)
