[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SignatureHelpProvider

# Interface: SignatureHelpProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).SignatureHelpProvider

## Table of contents

### Methods

- [provideSignatureHelp](codearts_plugin_.SignatureHelpProvider.md#providesignaturehelp)

## Methods

### provideSignatureHelp

▸ **provideSignatureHelp**(`document`, `position`, `token`, `context`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SignatureHelp`](../classes/codearts_plugin_.SignatureHelp.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |
| `context` | [`SignatureHelpContext`](codearts_plugin_.SignatureHelpContext.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SignatureHelp`](../classes/codearts_plugin_.SignatureHelp.md)\>

#### Defined in

[index.d.ts:4157](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L4157)
