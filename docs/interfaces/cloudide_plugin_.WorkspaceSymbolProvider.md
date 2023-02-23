[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / WorkspaceSymbolProvider

# Interface: WorkspaceSymbolProvider<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).WorkspaceSymbolProvider

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`SymbolInformation`](../classes/cloudide_plugin_.SymbolInformation.md) = [`SymbolInformation`](../classes/cloudide_plugin_.SymbolInformation.md) |

## Table of contents

### Methods

- [provideWorkspaceSymbols](cloudide_plugin_.WorkspaceSymbolProvider.md#provideworkspacesymbols)
- [resolveWorkspaceSymbol](cloudide_plugin_.WorkspaceSymbolProvider.md#resolveworkspacesymbol)

## Methods

### provideWorkspaceSymbols

▸ **provideWorkspaceSymbols**(`query`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

Project-wide search for a symbol matching the given query string.

The query-parameter should be interpreted in a relaxed way as the editor will apply its own
highlighting and scoring on the results. A good rule of thumb is to match case-insensitive and to
simply check that the characters of query appear in their order in a candidate symbol. Don't use
prefix, substring, or similar strict matching.

To improve performance implementors can implement resolveWorkspaceSymbol and then provide
symbols with partial location-objects, without a range defined. The editor will then call
resolveWorkspaceSymbol for selected symbols only, e.g. when opening a workspace symbol.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `query` | `string` | A non-empty query string. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

An array of document highlights or a thenable that
resolves to such. The lack of a result can be signaled by
returning undefined, null, or an empty array.

#### Defined in

[index.d.ts:10786](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10786)

___

### resolveWorkspaceSymbol

▸ `Optional` **resolveWorkspaceSymbol**(`symbol`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

Given a symbol fill in its [location](#SymbolInformation.location). This method is called whenever a symbol
is selected in the UI. Providers can implement this method and return incomplete symbols from
[`provideWorkspaceSymbols`](#WorkspaceSymbolProvider.provideWorkspaceSymbols) which often helps to improve
performance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `symbol` | `T` | The symbol that is to be resolved. Guaranteed to be an instance of an object returned from an earlier call to `provideWorkspaceSymbols`. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

The resolved symbol or a thenable that resolves to that. When no result is returned,
the given `symbol` is used.

#### Defined in

[index.d.ts:10800](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10800)
