**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentRangeSemanticTokensProvider

# Interface: DocumentRangeSemanticTokensProvider

The document range semantic tokens provider interface defines the contract between extensions and
semantic tokens.

## Hierarchy

* **DocumentRangeSemanticTokensProvider**

## Index

### Methods

* [provideDocumentRangeSemanticTokens](_index_d_._plugin_.documentrangesemantictokensprovider.md#providedocumentrangesemantictokens)

## Methods

### provideDocumentRangeSemanticTokens

▸ **provideDocumentRangeSemanticTokens**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `range`: [Range](../classes/_index_d_._plugin_.range.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[SemanticTokens](../classes/_index_d_._plugin_.semantictokens.md)>

*Defined in [index.d.ts:3634](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3634)*

**`see`** [provideDocumentSemanticTokens](#DocumentSemanticTokensProvider.provideDocumentSemanticTokens).

#### Parameters:

Name | Type |
------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) |
`range` | [Range](../classes/_index_d_._plugin_.range.md) |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[SemanticTokens](../classes/_index_d_._plugin_.semantictokens.md)>
