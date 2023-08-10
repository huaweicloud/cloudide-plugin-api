[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomDocument

# Interface: CustomDocument

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomDocument

Represents a custom document used by a [`CustomEditorProvider`](codearts_plugin_.CustomEditorProvider.md).

Custom documents are only used within a given `CustomEditorProvider`. The lifecycle of a `CustomDocument` is
managed by the editor. When no more references remain to a `CustomDocument`, it is disposed of.

## Table of contents

### Properties

- [uri](codearts_plugin_.CustomDocument.md#uri)

### Methods

- [dispose](codearts_plugin_.CustomDocument.md#dispose)

## Properties

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The associated uri for this document.

#### Defined in

[index.d.ts:8861](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L8861)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose of the custom document.

This is invoked by the editor when there are no more references to a given `CustomDocument` (for example when
all editors associated with the document have been closed.)

#### Returns

`void`

#### Defined in

[index.d.ts:8869](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L8869)
