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

[index.d.ts:11291](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11291)

___

### rangeLength

• `Readonly` **rangeLength**: `number`

The length of the range that got replaced.

#### Defined in

[index.d.ts:11299](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11299)

___

### rangeOffset

• `Readonly` **rangeOffset**: `number`

The offset of the range that got replaced.

#### Defined in

[index.d.ts:11295](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11295)

___

### text

• `Readonly` **text**: `string`

The new text for the range.

#### Defined in

[index.d.ts:11303](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11303)
