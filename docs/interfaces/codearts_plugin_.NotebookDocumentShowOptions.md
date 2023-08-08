[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookDocumentShowOptions

# Interface: NotebookDocumentShowOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookDocumentShowOptions

Represents options to configure the behavior of showing a [notebook document](codearts_plugin_.NotebookDocument.md) in an [notebook editor](codearts_plugin_.NotebookEditor.md).

## Table of contents

### Properties

- [preserveFocus](codearts_plugin_.NotebookDocumentShowOptions.md#preservefocus)
- [preview](codearts_plugin_.NotebookDocumentShowOptions.md#preview)
- [selections](codearts_plugin_.NotebookDocumentShowOptions.md#selections)
- [viewColumn](codearts_plugin_.NotebookDocumentShowOptions.md#viewcolumn)

## Properties

### preserveFocus

• `Optional` `Readonly` **preserveFocus**: `boolean`

An optional flag that when `true` will stop the [notebook editor](codearts_plugin_.NotebookEditor.md) from taking focus.

#### Defined in

[index.d.ts:835](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L835)

___

### preview

• `Optional` `Readonly` **preview**: `boolean`

An optional flag that controls if an [notebook editor](codearts_plugin_.NotebookEditor.md)-tab shows as preview. Preview tabs will
be replaced and reused until set to stay - either explicitly or through editing. The default behaviour depends
on the `workbench.editor.enablePreview`-setting.

#### Defined in

[index.d.ts:842](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L842)

___

### selections

• `Optional` `Readonly` **selections**: readonly [`NotebookRange`](../classes/codearts_plugin_.NotebookRange.md)[]

An optional selection to apply for the document in the [notebook editor](codearts_plugin_.NotebookEditor.md).

#### Defined in

[index.d.ts:847](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L847)

___

### viewColumn

• `Optional` `Readonly` **viewColumn**: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)

An optional view column in which the [notebook editor](codearts_plugin_.NotebookEditor.md) should be shown.
The default is the [active](../enums/codearts_plugin_.ViewColumn.md#active), other values are adjusted to
be `Min(column, columnCount + 1)`, the [active](../enums/codearts_plugin_.ViewColumn.md#active)-column is
not adjusted. Use [`Beside`](../enums/codearts_plugin_.ViewColumn.md#beside) to open the
editor to the side of the currently active one.

#### Defined in

[index.d.ts:830](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L830)
