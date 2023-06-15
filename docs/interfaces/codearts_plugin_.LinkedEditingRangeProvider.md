[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / LinkedEditingRangeProvider

# Interface: LinkedEditingRangeProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).LinkedEditingRangeProvider

The linked editing range provider interface defines the contract between extensions and
the linked editing feature.

## Table of contents

### Methods

- [provideLinkedEditingRanges](codearts_plugin_.LinkedEditingRangeProvider.md#providelinkededitingranges)

## Methods

### provideLinkedEditingRanges

▸ **provideLinkedEditingRanges**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`LinkedEditingRanges`](../classes/codearts_plugin_.LinkedEditingRanges.md)\>

For a given position in a document, returns the range of the symbol at the position and all ranges
that have the same content. A change to one of the ranges can be applied to all other ranges if the new content
is valid. An optional word pattern can be returned with the result to describe valid contents.
If no result-specific word pattern is provided, the word pattern from the language configuration is used.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the provider was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the provider was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`LinkedEditingRanges`](../classes/codearts_plugin_.LinkedEditingRanges.md)\>

A list of ranges that can be edited together

#### Defined in

[index.d.ts:5436](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5436)
