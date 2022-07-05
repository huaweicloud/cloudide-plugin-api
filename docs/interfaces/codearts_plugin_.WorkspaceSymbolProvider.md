[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WorkspaceSymbolProvider

# Interface: WorkspaceSymbolProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).WorkspaceSymbolProvider

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `query` | `string` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Defined in

[index.d.ts:3323](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3323)

___

### resolveWorkspaceSymbol

▸ `Optional` **resolveWorkspaceSymbol**(`symbol`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `symbol` | `T` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Defined in

[index.d.ts:3337](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3337)
