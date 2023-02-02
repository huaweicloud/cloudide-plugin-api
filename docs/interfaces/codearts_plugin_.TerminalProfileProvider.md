[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TerminalProfileProvider

# Interface: TerminalProfileProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).TerminalProfileProvider

Provides a terminal profile for the contributed terminal profile when launched via the UI or
command.

## Table of contents

### Methods

- [provideTerminalProfile](codearts_plugin_.TerminalProfileProvider.md#provideterminalprofile)

## Methods

### provideTerminalProfile

▸ **provideTerminalProfile**(`token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TerminalProfile`](../classes/codearts_plugin_.TerminalProfile.md)\>

Provide the terminal profile.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token that indicates the result is no longer needed. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TerminalProfile`](../classes/codearts_plugin_.TerminalProfile.md)\>

The terminal profile.

#### Defined in

[index.d.ts:6656](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6656)
