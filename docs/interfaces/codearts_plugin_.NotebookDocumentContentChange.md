[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookDocumentContentChange

# Interface: NotebookDocumentContentChange

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookDocumentContentChange

Describes a structural change to a notebook document, e.g newly added and removed cells.

**`See`**

[NotebookDocumentChangeEvent](codearts_plugin_.NotebookDocumentChangeEvent.md)

## Table of contents

### Properties

- [addedCells](codearts_plugin_.NotebookDocumentContentChange.md#addedcells)
- [range](codearts_plugin_.NotebookDocumentContentChange.md#range)
- [removedCells](codearts_plugin_.NotebookDocumentContentChange.md#removedcells)

## Properties

### addedCells

• `Readonly` **addedCells**: readonly [`NotebookCell`](codearts_plugin_.NotebookCell.md)[]

Cells that have been added to the document.

#### Defined in

[index.d.ts:14037](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14037)

___

### range

• `Readonly` **range**: [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md)

The range at which cells have been either added or removed.

Note that no cells have been [removed](codearts_plugin_.NotebookDocumentContentChange.md#removedcells)
when this range is [empty](../classes/codearts_plugin_.NotebookRange.md#isempty).

#### Defined in

[index.d.ts:14032](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14032)

___

### removedCells

• `Readonly` **removedCells**: readonly [`NotebookCell`](codearts_plugin_.NotebookCell.md)[]

Cells that have been removed from the document.

#### Defined in

[index.d.ts:14042](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14042)
