[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookDocumentContentOptions

# Interface: NotebookDocumentContentOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookDocumentContentOptions

Notebook content options define what parts of a notebook are persisted. Note

For instance, a notebook serializer can opt-out of saving outputs and in that case the editor doesn't mark a
notebooks as [dirty](codearts_plugin_.NotebookDocument.md#isdirty) when its output has changed.

## Table of contents

### Properties

- [transientCellMetadata](codearts_plugin_.NotebookDocumentContentOptions.md#transientcellmetadata)
- [transientDocumentMetadata](codearts_plugin_.NotebookDocumentContentOptions.md#transientdocumentmetadata)
- [transientOutputs](codearts_plugin_.NotebookDocumentContentOptions.md#transientoutputs)

## Properties

### transientCellMetadata

• `Optional` **transientCellMetadata**: `Object`

Controls if a cell metadata property change event will trigger notebook document content
change events and if it will be used in the diff editor, defaults to false. If the
content provider doesn't persist a metadata property in the file document, it should be
set to true.

#### Index signature

▪ [key: `string`]: `boolean` \| `undefined`

#### Defined in

[index.d.ts:13801](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L13801)

___

### transientDocumentMetadata

• `Optional` **transientDocumentMetadata**: `Object`

Controls if a document metadata property change event will trigger notebook document
content change event and if it will be used in the diff editor, defaults to false. If the
content provider doesn't persist a metadata property in the file document, it should be
set to true.

#### Index signature

▪ [key: `string`]: `boolean` \| `undefined`

#### Defined in

[index.d.ts:13809](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L13809)

___

### transientOutputs

• `Optional` **transientOutputs**: `boolean`

Controls if output change events will trigger notebook document content change events and
if it will be used in the diff editor, defaults to false. If the content provider doesn't
persist the outputs in the file document, this should be set to true.

#### Defined in

[index.d.ts:13793](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L13793)
