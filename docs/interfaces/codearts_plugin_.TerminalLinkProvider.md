[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TerminalLinkProvider

# Interface: TerminalLinkProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).TerminalLinkProvider

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `link` | `T` |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`void`\>

#### Defined in

[index.d.ts:6582](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L6582)

___

### provideTerminalLinks

▸ **provideTerminalLinks**(`context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | [`TerminalLinkContext`](codearts_plugin_.TerminalLinkContext.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Defined in

[index.d.ts:6576](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L6576)
