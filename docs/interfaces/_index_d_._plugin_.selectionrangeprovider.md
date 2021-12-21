**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SelectionRangeProvider

# Interface: SelectionRangeProvider

## Hierarchy

* **SelectionRangeProvider**

## Index

### Methods

* [provideSelectionRanges](_index_d_._plugin_.selectionrangeprovider.md#provideselectionranges)

## Methods

### provideSelectionRanges

▸ **provideSelectionRanges**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `positions`: [Position](../classes/_index_d_._plugin_.position.md)[], `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[SelectionRange](../classes/_index_d_._plugin_.selectionrange.md)[]>

*Defined in [index.d.ts:4530](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4530)*

Provide selection ranges for the given positions.

Selection ranges should be computed individually and independent for each position. The editor will merge
and deduplicate ranges but providers must return hierarchies of selection ranges so that a range
is [contained](#Range.contains) by its parent.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`positions` | [Position](../classes/_index_d_._plugin_.position.md)[] | The positions at which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[SelectionRange](../classes/_index_d_._plugin_.selectionrange.md)[]>

Selection ranges or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.
