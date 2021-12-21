**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextDocumentChangeEvent

# Interface: TextDocumentChangeEvent

An event describing a transactional [document](#TextDocument) change.

## Hierarchy

* **TextDocumentChangeEvent**

## Index

### Properties

* [contentChanges](_index_d_._plugin_.textdocumentchangeevent.md#contentchanges)
* [document](_index_d_._plugin_.textdocumentchangeevent.md#document)

## Properties

### contentChanges

• `Readonly` **contentChanges**: ReadonlyArray\<[TextDocumentContentChangeEvent](_index_d_._plugin_.textdocumentcontentchangeevent.md)>

*Defined in [index.d.ts:9984](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9984)*

An array of content changes.

___

### document

• `Readonly` **document**: [TextDocument](_index_d_._plugin_.textdocument.md)

*Defined in [index.d.ts:9979](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9979)*

The affected document.
