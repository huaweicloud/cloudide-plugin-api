[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentRangeSemanticTokensProvider

# Interface: DocumentRangeSemanticTokensProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentRangeSemanticTokensProvider

The document range semantic tokens provider interface defines the contract between extensions and
semantic tokens.

## Table of contents

### Methods

- [provideDocumentRangeSemanticTokens](cloudide_plugin_.DocumentRangeSemanticTokensProvider.md#providedocumentrangesemantictokens)

## Methods

### provideDocumentRangeSemanticTokens

▸ **provideDocumentRangeSemanticTokens**(`document`, `range`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`SemanticTokens`](../classes/cloudide_plugin_.SemanticTokens.md)\>

**`See`**

[provideDocumentSemanticTokens](#DocumentSemanticTokensProvider.provideDocumentSemanticTokens).

#### Parameters

| Name | Type |
| :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) |
| `range` | [`Range`](../classes/cloudide_plugin_.Range.md) |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`SemanticTokens`](../classes/cloudide_plugin_.SemanticTokens.md)\>

#### Defined in

[index.d.ts:8758](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8758)
