[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TerminalLinkProvider

# Interface: TerminalLinkProvider<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TerminalLinkProvider

A provider that enables detection and handling of links within terminals.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`TerminalLink`](cloudide_plugin_.TerminalLink.md) = [`TerminalLink`](cloudide_plugin_.TerminalLink.md) |

## Table of contents

### Methods

- [handleTerminalLink](cloudide_plugin_.TerminalLinkProvider.md#handleterminallink)
- [provideTerminalLinks](cloudide_plugin_.TerminalLinkProvider.md#provideterminallinks)

## Methods

### handleTerminalLink

▸ **handleTerminalLink**(`link`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`void`\>

Handle an activated terminal link.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `link` | `T` | The link to handle. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`void`\>

#### Defined in

[index.d.ts:2922](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2922)

___

### provideTerminalLinks

▸ **provideTerminalLinks**(`context`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

Provide terminal links for the given context. Note that this can be called multiple times
even before previous calls resolve, make sure to not share global objects (eg. `RegExp`)
that could have problems when asynchronous usage may overlap.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | [`TerminalLinkContext`](cloudide_plugin_.TerminalLinkContext.md) | Information about what links are being provided for. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

A list of terminal links for the given line.

#### Defined in

[index.d.ts:2916](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2916)
