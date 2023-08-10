[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TerminalLinkProvider

# Interface: TerminalLinkProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).TerminalLinkProvider

A provider that enables detection and handling of links within terminals.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`TerminalLink`](../classes/codearts_plugin_.TerminalLink.md) = [`TerminalLink`](../classes/codearts_plugin_.TerminalLink.md) |

## Table of contents

### Methods

- [handleTerminalLink](codearts_plugin_.TerminalLinkProvider.md#handleterminallink)
- [provideTerminalLinks](codearts_plugin_.TerminalLinkProvider.md#provideterminallinks)

## Methods

### handleTerminalLink

▸ **handleTerminalLink**(`link`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`void`\>

Handle an activated terminal link.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `link` | `T` | The link to handle. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`void`\>

#### Defined in

[index.d.ts:6704](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6704)

___

### provideTerminalLinks

▸ **provideTerminalLinks**(`context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

Provide terminal links for the given context. Note that this can be called multiple times
even before previous calls resolve, make sure to not share global objects (eg. `RegExp`)
that could have problems when asynchronous usage may overlap.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | [`TerminalLinkContext`](codearts_plugin_.TerminalLinkContext.md) | Information about what links are being provided for. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

A list of terminal links for the given line.

#### Defined in

[index.d.ts:6698](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6698)
