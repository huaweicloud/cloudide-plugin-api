**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FoldingRangeProvider

# Interface: FoldingRangeProvider

The folding range provider interface defines the contract between extensions and
[Folding](https://code.visualstudio.com/docs/editor/codebasics#_folding) in the editor.

## Hierarchy

* **FoldingRangeProvider**

## Index

### Properties

* [onDidChangeFoldingRanges](_index_d_._plugin_.foldingrangeprovider.md#ondidchangefoldingranges)

### Methods

* [provideFoldingRanges](_index_d_._plugin_.foldingrangeprovider.md#providefoldingranges)

## Properties

### onDidChangeFoldingRanges

• `Optional` **onDidChangeFoldingRanges**: [Event](_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:4479](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4479)*

An optional event to signal that the folding ranges from this provider have changed.

## Methods

### provideFoldingRanges

▸ **provideFoldingRanges**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `context`: [FoldingContext](_index_d_._plugin_.foldingcontext.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[FoldingRange](../classes/_index_d_._plugin_.foldingrange.md)[]>

*Defined in [index.d.ts:4488](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4488)*

Returns a list of folding ranges or null and undefined if the provider
does not want to participate or was cancelled.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`context` | [FoldingContext](_index_d_._plugin_.foldingcontext.md) | Additional context information (for future use) |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token.  |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[FoldingRange](../classes/_index_d_._plugin_.foldingrange.md)[]>
