[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CompletionItemProvider

# Interface: CompletionItemProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CompletionItemProvider

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |
| `context` | [`CompletionContext`](codearts_plugin_.CompletionContext.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[] \| [`CompletionList`](../classes/codearts_plugin_.CompletionList.md)<`T`\>\>

#### Defined in

[index.d.ts:4486](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L4486)

___

### resolveCompletionItem

▸ `Optional` **resolveCompletionItem**(`item`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | `T` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Defined in

[index.d.ts:4507](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L4507)
