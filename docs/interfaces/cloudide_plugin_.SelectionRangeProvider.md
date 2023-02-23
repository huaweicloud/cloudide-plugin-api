[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SelectionRangeProvider

# Interface: SelectionRangeProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SelectionRangeProvider

## Table of contents

### Methods

- [provideSelectionRanges](cloudide_plugin_.SelectionRangeProvider.md#provideselectionranges)

## Methods

### provideSelectionRanges

▸ **provideSelectionRanges**(`document`, `positions`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`SelectionRange`](../classes/cloudide_plugin_.SelectionRange.md)[]\>

Provide selection ranges for the given positions.

Selection ranges should be computed individually and independent for each position. The editor will merge
and deduplicate ranges but providers must return hierarchies of selection ranges so that a range
is [contained](#Range.contains) by its parent.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `positions` | [`Position`](../classes/cloudide_plugin_.Position.md)[] | The positions at which the command was invoked. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`SelectionRange`](../classes/cloudide_plugin_.SelectionRange.md)[]\>

Selection ranges or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:11128](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11128)
