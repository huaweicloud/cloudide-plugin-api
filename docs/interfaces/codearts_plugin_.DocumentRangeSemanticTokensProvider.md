[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentRangeSemanticTokensProvider

# Interface: DocumentRangeSemanticTokensProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentRangeSemanticTokensProvider

The document range semantic tokens provider interface defines the contract between extensions and
semantic tokens.

## Table of contents

### Methods

- [provideDocumentRangeSemanticTokens](codearts_plugin_.DocumentRangeSemanticTokensProvider.md#providedocumentrangesemantictokens)

## Methods

### provideDocumentRangeSemanticTokens

▸ **provideDocumentRangeSemanticTokens**(`document`, `range`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SemanticTokens`](../classes/codearts_plugin_.SemanticTokens.md)\>

**`See`**

[provideDocumentSemanticTokens](codearts_plugin_.DocumentSemanticTokensProvider.md#providedocumentsemantictokens).

#### Parameters

| Name | Type |
| :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SemanticTokens`](../classes/codearts_plugin_.SemanticTokens.md)\>

#### Defined in

[index.d.ts:3941](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3941)
