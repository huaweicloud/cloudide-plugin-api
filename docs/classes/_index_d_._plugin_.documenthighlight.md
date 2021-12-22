**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentHighlight

# Class: DocumentHighlight

A document highlight is a range inside a text document which deserves
special attention. Usually a document highlight is visualized by changing
the background color of its range.

## Hierarchy

* **DocumentHighlight**

## Index

### Constructors

* [constructor](_index_d_._plugin_.documenthighlight.md#constructor)

### Properties

* [kind](_index_d_._plugin_.documenthighlight.md#kind)
* [range](_index_d_._plugin_.documenthighlight.md#range)

## Constructors

### constructor

\+ **new DocumentHighlight**(`range`: [Range](_index_d_._plugin_.range.md), `kind?`: [DocumentHighlightKind](../enums/_index_d_._plugin_.documenthighlightkind.md)): [DocumentHighlight](_index_d_._plugin_.documenthighlight.md)

*Defined in [index.d.ts:2824](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2824)*

Creates a new document highlight object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | The range the highlight applies to. |
`kind?` | [DocumentHighlightKind](../enums/_index_d_._plugin_.documenthighlightkind.md) | The highlight kind, default is [text](#DocumentHighlightKind.Text).  |

**Returns:** [DocumentHighlight](_index_d_._plugin_.documenthighlight.md)

## Properties

### kind

• `Optional` **kind**: [DocumentHighlightKind](../enums/_index_d_._plugin_.documenthighlightkind.md)

*Defined in [index.d.ts:2824](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2824)*

The highlight kind, default is [text](#DocumentHighlightKind.Text).

___

### range

•  **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:2819](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2819)*

The range this highlight applies to.
