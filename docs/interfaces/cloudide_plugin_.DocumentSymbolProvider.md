[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentSymbolProvider

# Interface: DocumentSymbolProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentSymbolProvider

The document symbol provider interface defines the contract between extensions and
the [go to symbol](https://code.visualstudio.com/docs/editor/editingevolved#_go-to-symbol)-feature.

## Table of contents

### Methods

- [provideDocumentSymbols](cloudide_plugin_.DocumentSymbolProvider.md#providedocumentsymbols)

## Methods

### provideDocumentSymbols

▸ **provideDocumentSymbols**(`document`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DocumentSymbol`](../classes/cloudide_plugin_.DocumentSymbol.md)[] \| [`SymbolInformation`](../classes/cloudide_plugin_.SymbolInformation.md)[]\>

Provide symbol information for the given document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DocumentSymbol`](../classes/cloudide_plugin_.DocumentSymbol.md)[] \| [`SymbolInformation`](../classes/cloudide_plugin_.SymbolInformation.md)[]\>

An array of document highlights or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:7102](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7102)
