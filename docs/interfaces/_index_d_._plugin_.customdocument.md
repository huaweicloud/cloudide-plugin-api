**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CustomDocument

# Interface: CustomDocument

Represents a custom document used by a [`CustomEditorProvider`](#CustomEditorProvider).

Custom documents are only used within a given `CustomEditorProvider`. The lifecycle of a `CustomDocument` is
managed by VS Code. When no more references remain to a `CustomDocument`, it is disposed of.

## Hierarchy

* **CustomDocument**

## Index

### Properties

* [uri](_index_d_._plugin_.customdocument.md#uri)

### Methods

* [dispose](_index_d_._plugin_.customdocument.md#dispose)

## Properties

### uri

• `Readonly` **uri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:7679](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7679)*

The associated uri for this document.

## Methods

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:7687](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7687)*

Dispose of the custom document.

This is invoked by VS Code when there are no more references to a given `CustomDocument` (for example when
all editors associated with the document have been closed.)

**Returns:** void
