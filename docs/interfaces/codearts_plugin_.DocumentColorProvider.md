[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentColorProvider

# Interface: DocumentColorProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentColorProvider

The document color provider defines the contract between extensions and feature of
picking and modifying colors in the editor.

## Table of contents

### Methods

- [provideColorPresentations](codearts_plugin_.DocumentColorProvider.md#providecolorpresentations)
- [provideDocumentColors](codearts_plugin_.DocumentColorProvider.md#providedocumentcolors)

## Methods

### provideColorPresentations

▸ **provideColorPresentations**(`color`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`ColorPresentation`](../classes/codearts_plugin_.ColorPresentation.md)[]\>

Provide [representations](../classes/codearts_plugin_.ColorPresentation.md) for a color.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color` | [`Color`](../classes/codearts_plugin_.Color.md) | The color to show and insert. |
| `context` | `Object` | A context object with additional information |
| `context.document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | - |
| `context.range` | [`Range`](../classes/codearts_plugin_.Range.md) | - |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`ColorPresentation`](../classes/codearts_plugin_.ColorPresentation.md)[]\>

An array of color presentations or a thenable that resolves to such. The lack of a result
can be signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:4834](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L4834)

___

### provideDocumentColors

▸ **provideDocumentColors**(`document`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`ColorInformation`](../classes/codearts_plugin_.ColorInformation.md)[]\>

Provide colors for the given document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`ColorInformation`](../classes/codearts_plugin_.ColorInformation.md)[]\>

An array of [color information](../classes/codearts_plugin_.ColorInformation.md) or a thenable that resolves to such. The lack of a result
can be signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:4823](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L4823)
