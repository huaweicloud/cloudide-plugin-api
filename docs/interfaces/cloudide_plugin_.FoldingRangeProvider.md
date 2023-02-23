[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FoldingRangeProvider

# Interface: FoldingRangeProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FoldingRangeProvider

The folding range provider interface defines the contract between extensions and
[Folding](https://code.visualstudio.com/docs/editor/codebasics#_folding) in the editor.

## Table of contents

### Methods

- [provideFoldingRanges](cloudide_plugin_.FoldingRangeProvider.md#providefoldingranges)

## Methods

### provideFoldingRanges

▸ **provideFoldingRanges**(`document`, `context`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`FoldingRange`](../classes/cloudide_plugin_.FoldingRange.md)[]\>

Returns a list of folding ranges or null and undefined if the provider
does not want to participate or was cancelled.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `context` | [`FoldingContext`](cloudide_plugin_.FoldingContext.md) | Additional context information (for future use) |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`FoldingRange`](../classes/cloudide_plugin_.FoldingRange.md)[]\>

#### Defined in

[index.d.ts:7307](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7307)
