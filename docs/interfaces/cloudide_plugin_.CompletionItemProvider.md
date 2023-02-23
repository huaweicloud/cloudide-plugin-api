[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CompletionItemProvider

# Interface: CompletionItemProvider<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CompletionItemProvider

The completion item provider interface defines the contract between plugin and IntelliSense

Providers can delay the computation of the [`detail`](#CompletionItem.detail)
and [`documentation`](#CompletionItem.documentation) properties by implementing the
[`resolveCompletionItem`](#CompletionItemProvider.resolveCompletionItem)-function. However, properties that
are needed for the initial sorting and filtering, like `sortText`, `filterText`, `insertText`, and `range`, must
not be changed during resolve.

Providers are asked for completions either explicitly by a user gesture or -depending on the configuration-
implicitly when typing words or trigger characters.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CompletionItem`](../classes/cloudide_plugin_.CompletionItem.md) = [`CompletionItem`](../classes/cloudide_plugin_.CompletionItem.md) |

## Table of contents

### Methods

- [provideCompletionItems](cloudide_plugin_.CompletionItemProvider.md#providecompletionitems)
- [resolveCompletionItem](cloudide_plugin_.CompletionItemProvider.md#resolvecompletionitem)

## Methods

### provideCompletionItems

▸ **provideCompletionItems**(`document`, `position`, `token`, `context`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[] \| [`CompletionList`](../classes/cloudide_plugin_.CompletionList.md)<`T`\>\>

Provide completion items for the given position and document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |
| `context` | [`CompletionContext`](cloudide_plugin_.CompletionContext.md) | How the completion was triggered. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[] \| [`CompletionList`](../classes/cloudide_plugin_.CompletionList.md)<`T`\>\>

An array of completions, a [completion list](#CompletionList), or a thenable that resolves to either.
The lack of a result can be signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:7648](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7648)

___

### resolveCompletionItem

▸ `Optional` **resolveCompletionItem**(`item`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

Given a completion item fill in more data, like [doc-comment](#CompletionItem.documentation)
or [details](#CompletionItem.detail).

The editor will only resolve a completion item once.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | `T` | A completion item currently active in the UI. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

The resolved completion item or a thenable that resolves to of such. It is OK to return the given
`item`. When no result is returned, the given `item` will be used.

#### Defined in

[index.d.ts:7664](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7664)
