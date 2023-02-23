[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentFormattingEditProvider

# Interface: DocumentFormattingEditProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentFormattingEditProvider

The document formatting provider interface defines the contract between extensions and
the formatting-feature.

## Table of contents

### Methods

- [provideDocumentFormattingEdits](cloudide_plugin_.DocumentFormattingEditProvider.md#providedocumentformattingedits)

## Methods

### provideDocumentFormattingEdits

▸ **provideDocumentFormattingEdits**(`document`, `options`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`undefined` \| [`TextEdit`](../classes/cloudide_plugin_.TextEdit.md)[]\>

Provide formatting edits for a whole document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `options` | [`FormattingOptions`](cloudide_plugin_.FormattingOptions.md) | Options controlling formatting. |
| `token` | `undefined` \| [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`undefined` \| [`TextEdit`](../classes/cloudide_plugin_.TextEdit.md)[]\>

A set of text edits or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:8354](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8354)
