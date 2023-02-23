[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentHighlight

# Class: DocumentHighlight

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentHighlight

A document highlight is a range inside a text document which deserves
special attention. Usually a document highlight is visualized by changing
the background color of its range.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.DocumentHighlight.md#constructor)

### Properties

- [kind](cloudide_plugin_.DocumentHighlight.md#kind)
- [range](cloudide_plugin_.DocumentHighlight.md#range)

## Constructors

### constructor

• **new DocumentHighlight**(`range`, `kind?`)

Creates a new document highlight object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | The range the highlight applies to. |
| `kind?` | [`DocumentHighlightKind`](../enums/cloudide_plugin_.DocumentHighlightKind.md) | The highlight kind, default is [text](#DocumentHighlightKind.Text). |

#### Defined in

[index.d.ts:9291](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9291)

## Properties

### kind

• `Optional` **kind**: [`DocumentHighlightKind`](../enums/cloudide_plugin_.DocumentHighlightKind.md)

The highlight kind, default is [text](#DocumentHighlightKind.Text).

#### Defined in

[index.d.ts:9283](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9283)

___

### range

• **range**: [`Range`](cloudide_plugin_.Range.md)

The range this highlight applies to.

#### Defined in

[index.d.ts:9278](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9278)
