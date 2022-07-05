[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentHighlightProvider

# Interface: DocumentHighlightProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentHighlightProvider

## Table of contents

### Methods

- [provideDocumentHighlights](codearts_plugin_.DocumentHighlightProvider.md#providedocumenthighlights)

## Methods

### provideDocumentHighlights

▸ **provideDocumentHighlights**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DocumentHighlight`](../classes/codearts_plugin_.DocumentHighlight.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DocumentHighlight`](../classes/codearts_plugin_.DocumentHighlight.md)[]\>

#### Defined in

[index.d.ts:3117](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3117)
