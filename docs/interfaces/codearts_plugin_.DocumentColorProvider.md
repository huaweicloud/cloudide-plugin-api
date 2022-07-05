[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentColorProvider

# Interface: DocumentColorProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentColorProvider

## Table of contents

### Methods

- [provideColorPresentations](codearts_plugin_.DocumentColorProvider.md#providecolorpresentations)
- [provideDocumentColors](codearts_plugin_.DocumentColorProvider.md#providedocumentcolors)

## Methods

### provideColorPresentations

▸ **provideColorPresentations**(`color`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`ColorPresentation`](../classes/codearts_plugin_.ColorPresentation.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color` | [`Color`](../classes/codearts_plugin_.Color.md) |  |
| `context` | `Object` |  |
| `context.document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | - |
| `context.range` | [`Range`](../classes/codearts_plugin_.Range.md) | - |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`ColorPresentation`](../classes/codearts_plugin_.ColorPresentation.md)[]\>

#### Defined in

[index.d.ts:4834](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L4834)

___

### provideDocumentColors

▸ **provideDocumentColors**(`document`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`ColorInformation`](../classes/codearts_plugin_.ColorInformation.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`ColorInformation`](../classes/codearts_plugin_.ColorInformation.md)[]\>

#### Defined in

[index.d.ts:4823](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L4823)
