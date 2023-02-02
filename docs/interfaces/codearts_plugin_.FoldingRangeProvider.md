[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FoldingRangeProvider

# Interface: FoldingRangeProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).FoldingRangeProvider

The folding range provider interface defines the contract between extensions and
[Folding](https://code.visualstudio.com/docs/editor/codebasics#_folding) in the editor.

## Table of contents

### Properties

- [onDidChangeFoldingRanges](codearts_plugin_.FoldingRangeProvider.md#ondidchangefoldingranges)

### Methods

- [provideFoldingRanges](codearts_plugin_.FoldingRangeProvider.md#providefoldingranges)

## Properties

### onDidChangeFoldingRanges

• `Optional` **onDidChangeFoldingRanges**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An optional event to signal that the folding ranges from this provider have changed.

#### Defined in

[index.d.ts:5100](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5100)

## Methods

### provideFoldingRanges

▸ **provideFoldingRanges**(`document`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`FoldingRange`](../classes/codearts_plugin_.FoldingRange.md)[]\>

Returns a list of folding ranges or null and undefined if the provider
does not want to participate or was cancelled.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `context` | [`FoldingContext`](codearts_plugin_.FoldingContext.md) | Additional context information (for future use) |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`FoldingRange`](../classes/codearts_plugin_.FoldingRange.md)[]\>

#### Defined in

[index.d.ts:5109](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5109)
