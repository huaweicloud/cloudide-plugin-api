[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentFormattingEditProvider

# Interface: DocumentFormattingEditProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentFormattingEditProvider

The document formatting provider interface defines the contract between extensions and
the formatting-feature.

## Table of contents

### Methods

- [provideDocumentFormattingEdits](codearts_plugin_.DocumentFormattingEditProvider.md#providedocumentformattingedits)

## Methods

### provideDocumentFormattingEdits

▸ **provideDocumentFormattingEdits**(`document`, `options`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

Provide formatting edits for a whole document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `options` | [`FormattingOptions`](codearts_plugin_.FormattingOptions.md) | Options controlling formatting. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

A set of text edits or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:3980](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3980)
