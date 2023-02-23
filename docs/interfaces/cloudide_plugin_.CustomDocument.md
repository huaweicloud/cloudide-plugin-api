[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CustomDocument

# Interface: CustomDocument

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CustomDocument

Represents a custom document used by a [`CustomEditorProvider`](#CustomEditorProvider).

Custom documents are only used within a given `CustomEditorProvider`. The lifecycle of a `CustomDocument` is
managed by Theia. When no more references remain to a `CustomDocument`, it is disposed of.

## Table of contents

### Properties

- [uri](cloudide_plugin_.CustomDocument.md#uri)

### Methods

- [dispose](cloudide_plugin_.CustomDocument.md#dispose)

## Properties

### uri

• `Readonly` **uri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The associated uri for this document.

#### Defined in

[index.d.ts:3772](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3772)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose of the custom document.

This is invoked by Theia when there are no more references to a given `CustomDocument` (for example when
all editors associated with the document have been closed.)

#### Returns

`void`

#### Defined in

[index.d.ts:3780](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3780)
