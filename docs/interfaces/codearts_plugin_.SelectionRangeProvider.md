[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SelectionRangeProvider

# Interface: SelectionRangeProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).SelectionRangeProvider

## Table of contents

### Methods

- [provideSelectionRanges](codearts_plugin_.SelectionRangeProvider.md#provideselectionranges)

## Methods

### provideSelectionRanges

▸ **provideSelectionRanges**(`document`, `positions`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SelectionRange`](../classes/codearts_plugin_.SelectionRange.md)[]\>

Provide selection ranges for the given positions.

Selection ranges should be computed individually and independent for each position. The editor will merge
and deduplicate ranges but providers must return hierarchies of selection ranges so that a range
is [contained](../classes/codearts_plugin_.Range.md#contains) by its parent.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `positions` | readonly [`Position`](../classes/codearts_plugin_.Position.md)[] | The positions at which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SelectionRange`](../classes/codearts_plugin_.SelectionRange.md)[]\>

Selection ranges or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:5151](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5151)
