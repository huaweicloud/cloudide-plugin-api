[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookEditorVisibleRangesChangeEvent

# Interface: NotebookEditorVisibleRangesChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookEditorVisibleRangesChangeEvent

Represents an event describing the change in a [notebook editor's visibleRanges](codearts_plugin_.NotebookEditor.md#visibleranges).

## Table of contents

### Properties

- [notebookEditor](codearts_plugin_.NotebookEditorVisibleRangesChangeEvent.md#notebookeditor)
- [visibleRanges](codearts_plugin_.NotebookEditorVisibleRangesChangeEvent.md#visibleranges)

## Properties

### notebookEditor

• `Readonly` **notebookEditor**: [`NotebookEditor`](codearts_plugin_.NotebookEditor.md)

The [notebook editor](codearts_plugin_.NotebookEditor.md) for which the visible ranges have changed.

#### Defined in

[index.d.ts:811](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L811)

___

### visibleRanges

• `Readonly` **visibleRanges**: readonly [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md)[]

The new value for the [notebook editor's visibleRanges](codearts_plugin_.NotebookEditor.md#visibleranges).

#### Defined in

[index.d.ts:816](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L816)
