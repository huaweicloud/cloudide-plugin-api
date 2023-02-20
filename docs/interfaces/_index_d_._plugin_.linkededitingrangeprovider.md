**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / LinkedEditingRangeProvider

# Interface: LinkedEditingRangeProvider

The linked editing range provider interface defines the contract between extensions and
the linked editing feature.

## Hierarchy

* **LinkedEditingRangeProvider**

## Index

### Methods

* [provideLinkedEditingRanges](_index_d_._plugin_.linkededitingrangeprovider.md#providelinkededitingranges)

## Methods

### provideLinkedEditingRanges

▸ **provideLinkedEditingRanges**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[LinkedEditingRanges](../classes/_index_d_._plugin_.linkededitingranges.md)>

*Defined in [index.d.ts:4720](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4720)*

For a given position in a document, returns the range of the symbol at the position and all ranges
that have the same content. A change to one of the ranges can be applied to all other ranges if the new content
is valid. An optional word pattern can be returned with the result to describe valid contents.
If no result-specific word pattern is provided, the word pattern from the language configuration is used.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the provider was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the provider was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[LinkedEditingRanges](../classes/_index_d_._plugin_.linkededitingranges.md)>

A list of ranges that can be edited together
