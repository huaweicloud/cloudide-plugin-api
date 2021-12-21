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

*Defined in [index.d.ts:9956](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9956)*

The range that got replaced.

___

### rangeLength

• `Readonly` **rangeLength**: number

*Defined in [index.d.ts:9964](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9964)*

The length of the range that got replaced.

___

### rangeOffset

• `Readonly` **rangeOffset**: number

*Defined in [index.d.ts:9960](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9960)*

The offset of the range that got replaced.

___

### text

• `Readonly` **text**: string

*Defined in [index.d.ts:9968](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9968)*

The new text for the range.
