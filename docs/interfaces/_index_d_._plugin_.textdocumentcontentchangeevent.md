**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextDocumentContentChangeEvent

# Interface: TextDocumentContentChangeEvent

An event describing an individual change in the text of a [document](#TextDocument).

## Hierarchy

* **TextDocumentContentChangeEvent**

## Index

### Properties

* [range](_index_d_._plugin_.textdocumentcontentchangeevent.md#range)
* [rangeLength](_index_d_._plugin_.textdocumentcontentchangeevent.md#rangelength)
* [rangeOffset](_index_d_._plugin_.textdocumentcontentchangeevent.md#rangeoffset)
* [text](_index_d_._plugin_.textdocumentcontentchangeevent.md#text)

## Properties

### range

• `Readonly` **range**: [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:10008](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L10008)*

The range that got replaced.

___

### rangeLength

• `Readonly` **rangeLength**: number

*Defined in [index.d.ts:10016](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L10016)*

The length of the range that got replaced.

___

### rangeOffset

• `Readonly` **rangeOffset**: number

*Defined in [index.d.ts:10012](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L10012)*

The offset of the range that got replaced.

___

### text

• `Readonly` **text**: string

*Defined in [index.d.ts:10020](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L10020)*

The new text for the range.
