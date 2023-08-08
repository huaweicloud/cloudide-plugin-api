[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentHighlight

# Class: DocumentHighlight

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentHighlight

A document highlight is a range inside a text document which deserves
special attention. Usually a document highlight is visualized by changing
the background color of its range.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.DocumentHighlight.md#constructor)

### Properties

- [kind](codearts_plugin_.DocumentHighlight.md#kind)
- [range](codearts_plugin_.DocumentHighlight.md#range)

## Constructors

### constructor

• **new DocumentHighlight**(`range`, `kind?`)

Creates a new document highlight object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The range the highlight applies to. |
| `kind?` | [`DocumentHighlightKind`](../enums/codearts_plugin_.DocumentHighlightKind.md) | The highlight kind, default is [text](../enums/codearts_plugin_.DocumentHighlightKind.md#text). |

#### Defined in

[index.d.ts:3098](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3098)

## Properties

### kind

• `Optional` **kind**: [`DocumentHighlightKind`](../enums/codearts_plugin_.DocumentHighlightKind.md)

The highlight kind, default is [text](../enums/codearts_plugin_.DocumentHighlightKind.md#text).

#### Defined in

[index.d.ts:3090](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3090)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The range this highlight applies to.

#### Defined in

[index.d.ts:3085](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3085)
