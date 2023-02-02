[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentHighlightProvider

# Interface: DocumentHighlightProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentHighlightProvider

The document highlight provider interface defines the contract between extensions and
the word-highlight-feature.

## Table of contents

### Methods

- [provideDocumentHighlights](codearts_plugin_.DocumentHighlightProvider.md#providedocumenthighlights)

## Methods

### provideDocumentHighlights

▸ **provideDocumentHighlights**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DocumentHighlight`](../classes/codearts_plugin_.DocumentHighlight.md)[]\>

Provide a set of document highlights, like all occurrences of a variable or
all exit-points of a function.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DocumentHighlight`](../classes/codearts_plugin_.DocumentHighlight.md)[]\>

An array of document highlights or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:3117](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L3117)
