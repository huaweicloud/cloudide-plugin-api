[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextDocumentContentChangeEvent

# Interface: TextDocumentContentChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextDocumentContentChangeEvent

An event describing an individual change in the text of a [document](codearts_plugin_.TextDocument.md).

## Table of contents

### Properties

- [range](codearts_plugin_.TextDocumentContentChangeEvent.md#range)
- [rangeLength](codearts_plugin_.TextDocumentContentChangeEvent.md#rangelength)
- [rangeOffset](codearts_plugin_.TextDocumentContentChangeEvent.md#rangeoffset)
- [text](codearts_plugin_.TextDocumentContentChangeEvent.md#text)

## Properties

### range

• `Readonly` **range**: [`Range`](../classes/codearts_plugin_.Range.md)

The range that got replaced.

#### Defined in

[index.d.ts:11700](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L11700)

___

### rangeLength

• `Readonly` **rangeLength**: `number`

The length of the range that got replaced.

#### Defined in

[index.d.ts:11708](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L11708)

___

### rangeOffset

• `Readonly` **rangeOffset**: `number`

The offset of the range that got replaced.

#### Defined in

[index.d.ts:11704](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L11704)

___

### text

• `Readonly` **text**: `string`

The new text for the range.

#### Defined in

[index.d.ts:11712](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L11712)
