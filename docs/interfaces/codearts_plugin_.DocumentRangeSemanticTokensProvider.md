[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentRangeSemanticTokensProvider

# Interface: DocumentRangeSemanticTokensProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentRangeSemanticTokensProvider

## Table of contents

### Methods

- [provideDocumentRangeSemanticTokens](codearts_plugin_.DocumentRangeSemanticTokensProvider.md#providedocumentrangesemantictokens)

## Methods

### provideDocumentRangeSemanticTokens

▸ **provideDocumentRangeSemanticTokens**(`document`, `range`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SemanticTokens`](../classes/codearts_plugin_.SemanticTokens.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SemanticTokens`](../classes/codearts_plugin_.SemanticTokens.md)\>

#### Defined in

[index.d.ts:3903](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3903)
