**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SignatureHelpProvider

# Interface: SignatureHelpProvider

The signature help provider interface defines the contract between extensions and
the [parameter hints](https://code.visualstudio.com/docs/editor/intellisense)-feature.

## Hierarchy

* **SignatureHelpProvider**

## Index

### Methods

* [provideSignatureHelp](_index_d_._plugin_.signaturehelpprovider.md#providesignaturehelp)

## Methods

### provideSignatureHelp

▸ **provideSignatureHelp**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md), `context`: [SignatureHelpContext](_index_d_._plugin_.signaturehelpcontext.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[SignatureHelp](../classes/_index_d_._plugin_.signaturehelp.md)>

*Defined in [index.d.ts:3891](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3891)*

Provide help for the signature at the given position and document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |
`context` | [SignatureHelpContext](_index_d_._plugin_.signaturehelpcontext.md) | Information about how signature help was triggered.  |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[SignatureHelp](../classes/_index_d_._plugin_.signaturehelp.md)>

Signature help or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.
