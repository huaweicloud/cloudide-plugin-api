[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentSymbolProvider

# Interface: DocumentSymbolProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentSymbolProvider

## Table of contents

### Methods

- [provideDocumentSymbols](codearts_plugin_.DocumentSymbolProvider.md#providedocumentsymbols)

## Methods

### provideDocumentSymbols

▸ **provideDocumentSymbols**(`document`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DocumentSymbol`](../classes/codearts_plugin_.DocumentSymbol.md)[] \| [`SymbolInformation`](../classes/codearts_plugin_.SymbolInformation.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DocumentSymbol`](../classes/codearts_plugin_.DocumentSymbol.md)[] \| [`SymbolInformation`](../classes/codearts_plugin_.SymbolInformation.md)[]\>

#### Defined in

[index.d.ts:3287](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3287)
