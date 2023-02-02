[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CompletionItemProvider

# Interface: CompletionItemProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CompletionItemProvider

The completion item provider interface defines the contract between extensions and
[IntelliSense](https://code.visualstudio.com/docs/editor/intellisense).

Providers can delay the computation of the [`detail`](../classes/codearts_plugin_.CompletionItem.md#detail)
and [`documentation`](../classes/codearts_plugin_.CompletionItem.md#documentation) properties by implementing the
[`resolveCompletionItem`](codearts_plugin_.CompletionItemProvider.md#resolvecompletionitem)-function. However, properties that
are needed for the initial sorting and filtering, like `sortText`, `filterText`, `insertText`, and `range`, must
not be changed during resolve.

Providers are asked for completions either explicitly by a user gesture or -depending on the configuration-
implicitly when typing words or trigger characters.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CompletionItem`](../classes/codearts_plugin_.CompletionItem.md) = [`CompletionItem`](../classes/codearts_plugin_.CompletionItem.md) |

## Table of contents

### Methods

- [provideCompletionItems](codearts_plugin_.CompletionItemProvider.md#providecompletionitems)
- [resolveCompletionItem](codearts_plugin_.CompletionItemProvider.md#resolvecompletionitem)

## Methods

### provideCompletionItems

▸ **provideCompletionItems**(`document`, `position`, `token`, `context`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[] \| [`CompletionList`](../classes/codearts_plugin_.CompletionList.md)<`T`\>\>

Provide completion items for the given position and document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |
| `context` | [`CompletionContext`](codearts_plugin_.CompletionContext.md) | How the completion was triggered. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[] \| [`CompletionList`](../classes/codearts_plugin_.CompletionList.md)<`T`\>\>

An array of completions, a [completion list](../classes/codearts_plugin_.CompletionList.md), or a thenable that resolves to either.
The lack of a result can be signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:4506](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4506)

___

### resolveCompletionItem

▸ `Optional` **resolveCompletionItem**(`item`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

Given a completion item fill in more data, like [doc-comment](../classes/codearts_plugin_.CompletionItem.md#documentation)
or [details](../classes/codearts_plugin_.CompletionItem.md#detail).

The editor will only resolve a completion item once.

*Note* that this function is called when completion items are already showing in the UI or when an item has been
selected for insertion. Because of that, no property that changes the presentation (label, sorting, filtering etc)
or the (primary) insert behaviour ([insertText](../classes/codearts_plugin_.CompletionItem.md#inserttext)) can be changed.

This function may fill in [additionalTextEdits](../classes/codearts_plugin_.CompletionItem.md#additionaltextedits). However, that means an item might be
inserted *before* resolving is done and in that case the editor will do a best effort to still apply those additional
text edits.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | `T` | A completion item currently active in the UI. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

The resolved completion item or a thenable that resolves to of such. It is OK to return the given
`item`. When no result is returned, the given `item` will be used.

#### Defined in

[index.d.ts:4527](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4527)
