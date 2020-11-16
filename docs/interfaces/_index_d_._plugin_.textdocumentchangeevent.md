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

*Defined in [index.d.ts:8646](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8646)*

An array of content changes.

___

### document

• `Readonly` **document**: [TextDocument](_index_d_._plugin_.textdocument.md)

*Defined in [index.d.ts:8641](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8641)*

The affected document.
