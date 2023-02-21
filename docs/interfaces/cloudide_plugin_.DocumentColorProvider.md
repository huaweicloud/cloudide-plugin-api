[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentColorProvider

# Interface: DocumentColorProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentColorProvider

The document color provider defines the contract between extensions and feature of
picking and modifying colors in the editor.

## Table of contents

### Methods

- [provideColorPresentations](cloudide_plugin_.DocumentColorProvider.md#providecolorpresentations)
- [provideDocumentColors](cloudide_plugin_.DocumentColorProvider.md#providedocumentcolors)

## Methods

### provideColorPresentations

▸ **provideColorPresentations**(`color`, `context`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`ColorPresentation`](../classes/cloudide_plugin_.ColorPresentation.md)[]\>

Provide [representations](#ColorPresentation) for a color.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color` | [`Color`](../classes/cloudide_plugin_.Color.md) | The color to show and insert. |
| `context` | `Object` | A context object with additional information |
| `context.document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | - |
| `context.range` | [`Range`](../classes/cloudide_plugin_.Range.md) | - |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`ColorPresentation`](../classes/cloudide_plugin_.ColorPresentation.md)[]\>

An array of color presentations or a thenable that resolves to such. The lack of a result
can be signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:7228](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7228)

___

### provideDocumentColors

▸ **provideDocumentColors**(`document`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`ColorInformation`](../classes/cloudide_plugin_.ColorInformation.md)[]\>

Provide colors for the given document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`ColorInformation`](../classes/cloudide_plugin_.ColorInformation.md)[]\>

An array of [color information](#ColorInformation) or a thenable that resolves to such. The lack of a result
can be signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:7217](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7217)
