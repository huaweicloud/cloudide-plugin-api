**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentSymbolProvider

# Interface: DocumentSymbolProvider

The document symbol provider interface defines the contract between extensions and
the [go to symbol](https://code.visualstudio.com/docs/editor/editingevolved#_go-to-symbol)-feature.

## Hierarchy

* **DocumentSymbolProvider**

## Index

### Methods

* [provideDocumentSymbols](_index_d_._plugin_.documentsymbolprovider.md#providedocumentsymbols)

## Methods

### provideDocumentSymbols

▸ **provideDocumentSymbols**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[SymbolInformation](../classes/_index_d_._plugin_.symbolinformation.md)[] \| [DocumentSymbol](../classes/_index_d_._plugin_.documentsymbol.md)[]>

*Defined in [index.d.ts:2792](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2792)*

Provide symbol information for the given document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[SymbolInformation](../classes/_index_d_._plugin_.symbolinformation.md)[] \| [DocumentSymbol](../classes/_index_d_._plugin_.documentsymbol.md)[]>

An array of document highlights or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.
