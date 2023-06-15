[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineCompletionItemProvider

# Interface: InlineCompletionItemProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineCompletionItemProvider

The inline completion item provider interface defines the contract between extensions and
the inline completion feature.

Providers are asked for completions either explicitly by a user gesture or implicitly when typing.

## Table of contents

### Methods

- [provideInlineCompletionItems](codearts_plugin_.InlineCompletionItemProvider.md#provideinlinecompletionitems)

## Methods

### provideInlineCompletionItems

▸ **provideInlineCompletionItems**(`document`, `position`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`InlineCompletionItem`](../classes/codearts_plugin_.InlineCompletionItem.md)[] \| [`InlineCompletionList`](../classes/codearts_plugin_.InlineCompletionList.md)\>

Provides inline completion items for the given position and document.
If inline completions are enabled, this method will be called whenever the user stopped typing.
It will also be called when the user explicitly triggers inline completions or explicitly asks for the next or previous inline completion.
In that case, all available inline completions should be returned.
`context.triggerKind` can be used to distinguish between these scenarios.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document inline completions are requested for. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position inline completions are requested for. |
| `context` | [`InlineCompletionContext`](codearts_plugin_.InlineCompletionContext.md) | A context object with additional information. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`InlineCompletionItem`](../classes/codearts_plugin_.InlineCompletionItem.md)[] \| [`InlineCompletionList`](../classes/codearts_plugin_.InlineCompletionList.md)\>

An array of completion items or a thenable that resolves to an array of completion items.

#### Defined in

[index.d.ts:4552](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L4552)
