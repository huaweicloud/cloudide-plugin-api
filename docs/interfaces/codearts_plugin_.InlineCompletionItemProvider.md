[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineCompletionItemProvider

# Interface: InlineCompletionItemProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineCompletionItemProvider

## Table of contents

### Methods

- [provideInlineCompletionItems](codearts_plugin_.InlineCompletionItemProvider.md#provideinlinecompletionitems)

## Methods

### provideInlineCompletionItems

▸ **provideInlineCompletionItems**(`document`, `position`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`InlineCompletionItem`](../classes/codearts_plugin_.InlineCompletionItem.md)[] \| [`InlineCompletionList`](../classes/codearts_plugin_.InlineCompletionList.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `context` | [`InlineCompletionContext`](codearts_plugin_.InlineCompletionContext.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`InlineCompletionItem`](../classes/codearts_plugin_.InlineCompletionItem.md)[] \| [`InlineCompletionList`](../classes/codearts_plugin_.InlineCompletionList.md)\>

#### Defined in

[index.d.ts:4532](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4532)
