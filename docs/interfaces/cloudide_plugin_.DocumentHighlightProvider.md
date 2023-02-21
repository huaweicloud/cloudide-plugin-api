[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentHighlightProvider

# Interface: DocumentHighlightProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentHighlightProvider

The document highlight provider interface defines the contract between extensions and
the word-highlight-feature.

## Table of contents

### Methods

- [provideDocumentHighlights](cloudide_plugin_.DocumentHighlightProvider.md#providedocumenthighlights)

## Methods

### provideDocumentHighlights

▸ **provideDocumentHighlights**(`document`, `position`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DocumentHighlight`](../classes/cloudide_plugin_.DocumentHighlight.md)[]\>

Provide a set of document highlights, like all occurrences of a variable or
all exit-points of a function.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | `undefined` \| [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DocumentHighlight`](../classes/cloudide_plugin_.DocumentHighlight.md)[]\>

An array of document highlights or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:9310](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9310)
