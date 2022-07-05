[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentSemanticTokensProvider

# Interface: DocumentSemanticTokensProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentSemanticTokensProvider

## Table of contents

### Properties

- [onDidChangeSemanticTokens](codearts_plugin_.DocumentSemanticTokensProvider.md#ondidchangesemantictokens)

### Methods

- [provideDocumentSemanticTokens](codearts_plugin_.DocumentSemanticTokensProvider.md#providedocumentsemantictokens)
- [provideDocumentSemanticTokensEdits](codearts_plugin_.DocumentSemanticTokensProvider.md#providedocumentsemantictokensedits)

## Properties

### onDidChangeSemanticTokens

• `Optional` **onDidChangeSemanticTokens**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:3800](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3800)

## Methods

### provideDocumentSemanticTokens

▸ **provideDocumentSemanticTokens**(`document`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SemanticTokens`](../classes/codearts_plugin_.SemanticTokens.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SemanticTokens`](../classes/codearts_plugin_.SemanticTokens.md)\>

#### Defined in

[index.d.ts:3861](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3861)

___

### provideDocumentSemanticTokensEdits

▸ `Optional` **provideDocumentSemanticTokensEdits**(`document`, `previousResultId`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SemanticTokens`](../classes/codearts_plugin_.SemanticTokens.md) \| [`SemanticTokensEdits`](../classes/codearts_plugin_.SemanticTokensEdits.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |
| `previousResultId` | `string` |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SemanticTokens`](../classes/codearts_plugin_.SemanticTokens.md) \| [`SemanticTokensEdits`](../classes/codearts_plugin_.SemanticTokensEdits.md)\>

#### Defined in

[index.d.ts:3892](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3892)
