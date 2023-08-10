[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SignatureHelpProvider

# Interface: SignatureHelpProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).SignatureHelpProvider

The signature help provider interface defines the contract between extensions and
the [parameter hints](https://code.visualstudio.com/docs/editor/intellisense)-feature.

## Table of contents

### Methods

- [provideSignatureHelp](codearts_plugin_.SignatureHelpProvider.md#providesignaturehelp)

## Methods

### provideSignatureHelp

▸ **provideSignatureHelp**(`document`, `position`, `token`, `context`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SignatureHelp`](../classes/codearts_plugin_.SignatureHelp.md)\>

Provide help for the signature at the given position and document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |
| `context` | [`SignatureHelpContext`](codearts_plugin_.SignatureHelpContext.md) | Information about how signature help was triggered. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SignatureHelp`](../classes/codearts_plugin_.SignatureHelp.md)\>

Signature help or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:4195](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4195)
