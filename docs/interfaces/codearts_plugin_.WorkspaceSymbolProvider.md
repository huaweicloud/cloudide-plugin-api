[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WorkspaceSymbolProvider

# Interface: WorkspaceSymbolProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).WorkspaceSymbolProvider

The workspace symbol provider interface defines the contract between extensions and
the [symbol search](https://code.visualstudio.com/docs/editor/editingevolved#_open-symbol-by-name)-feature.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`SymbolInformation`](../classes/codearts_plugin_.SymbolInformation.md) = [`SymbolInformation`](../classes/codearts_plugin_.SymbolInformation.md) |

## Table of contents

### Methods

- [provideWorkspaceSymbols](codearts_plugin_.WorkspaceSymbolProvider.md#provideworkspacesymbols)
- [resolveWorkspaceSymbol](codearts_plugin_.WorkspaceSymbolProvider.md#resolveworkspacesymbol)

## Methods

### provideWorkspaceSymbols

▸ **provideWorkspaceSymbols**(`query`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

Project-wide search for a symbol matching the given query string.

The `query`-parameter should be interpreted in a *relaxed way* as the editor will apply its own highlighting
and scoring on the results. A good rule of thumb is to match case-insensitive and to simply check that the
characters of *query* appear in their order in a candidate symbol. Don't use prefix, substring, or similar
strict matching.

To improve performance implementors can implement `resolveWorkspaceSymbol` and then provide symbols with partial
[location](../classes/codearts_plugin_.SymbolInformation.md#location)-objects, without a `range` defined. The editor will then call
`resolveWorkspaceSymbol` for selected symbols only, e.g. when opening a workspace symbol.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `query` | `string` | A query string, can be the empty string in which case all symbols should be returned. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

An array of document highlights or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:3323](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L3323)

___

### resolveWorkspaceSymbol

▸ `Optional` **resolveWorkspaceSymbol**(`symbol`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

Given a symbol fill in its [location](../classes/codearts_plugin_.SymbolInformation.md#location). This method is called whenever a symbol
is selected in the UI. Providers can implement this method and return incomplete symbols from
[`provideWorkspaceSymbols`](codearts_plugin_.WorkspaceSymbolProvider.md#provideworkspacesymbols) which often helps to improve
performance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `symbol` | `T` | The symbol that is to be resolved. Guaranteed to be an instance of an object returned from an earlier call to `provideWorkspaceSymbols`. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

The resolved symbol or a thenable that resolves to that. When no result is returned,
the given `symbol` is used.

#### Defined in

[index.d.ts:3337](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L3337)
