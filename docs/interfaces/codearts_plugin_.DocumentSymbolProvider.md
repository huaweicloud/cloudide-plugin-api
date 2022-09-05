[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentSymbolProvider

# Interface: DocumentSymbolProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentSymbolProvider

The document symbol provider interface defines the contract between extensions and
the [go to symbol](https://code.visualstudio.com/docs/editor/editingevolved#_go-to-symbol)-feature.

## Table of contents

### Methods

- [provideDocumentSymbols](codearts_plugin_.DocumentSymbolProvider.md#providedocumentsymbols)

## Methods

### provideDocumentSymbols

▸ **provideDocumentSymbols**(`document`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DocumentSymbol`](../classes/codearts_plugin_.DocumentSymbol.md)[] \| [`SymbolInformation`](../classes/codearts_plugin_.SymbolInformation.md)[]\>

Provide symbol information for the given document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DocumentSymbol`](../classes/codearts_plugin_.DocumentSymbol.md)[] \| [`SymbolInformation`](../classes/codearts_plugin_.SymbolInformation.md)[]\>

An array of document highlights or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:3287](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3287)
