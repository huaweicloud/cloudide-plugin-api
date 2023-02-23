[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / QuickDiffProvider

# Interface: QuickDiffProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).QuickDiffProvider

## Table of contents

### Methods

- [provideOriginalResource](cloudide_plugin_.QuickDiffProvider.md#provideoriginalresource)

## Methods

### provideOriginalResource

▸ `Optional` **provideOriginalResource**(`uri`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Uri`](../classes/cloudide_plugin_.Uri.md)\>

Provide a [uri](#Uri) to the original resource of any given resource uri.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the resource open in a text editor. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Uri`](../classes/cloudide_plugin_.Uri.md)\>

A thenable that resolves to uri of the matching original resource.

#### Defined in

[index.d.ts:9338](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9338)
