**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentColorProvider

# Interface: DocumentColorProvider

The document color provider defines the contract between extensions and feature of
picking and modifying colors in the editor.

## Hierarchy

* **DocumentColorProvider**

## Index

### Methods

* [provideColorPresentations](_index_d_._plugin_.documentcolorprovider.md#providecolorpresentations)
* [provideDocumentColors](_index_d_._plugin_.documentcolorprovider.md#providedocumentcolors)

## Methods

### provideColorPresentations

▸ **provideColorPresentations**(`color`: [Color](../classes/_index_d_._plugin_.color.md), `context`: { document: [TextDocument](_index_d_._plugin_.textdocument.md) ; range: [Range](../classes/_index_d_._plugin_.range.md)  }, `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[ColorPresentation](../classes/_index_d_._plugin_.colorpresentation.md)[]>

*Defined in [index.d.ts:4406](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4406)*

Provide [representations](#ColorPresentation) for a color.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`color` | [Color](../classes/_index_d_._plugin_.color.md) | The color to show and insert. |
`context` | { document: [TextDocument](_index_d_._plugin_.textdocument.md) ; range: [Range](../classes/_index_d_._plugin_.range.md)  } | A context object with additional information |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[ColorPresentation](../classes/_index_d_._plugin_.colorpresentation.md)[]>

An array of color presentations or a thenable that resolves to such. The lack of a result
can be signaled by returning `undefined`, `null`, or an empty array.

___

### provideDocumentColors

▸ **provideDocumentColors**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[ColorInformation](../classes/_index_d_._plugin_.colorinformation.md)[]>

*Defined in [index.d.ts:4395](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4395)*

Provide colors for the given document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[ColorInformation](../classes/_index_d_._plugin_.colorinformation.md)[]>

An array of [color information](#ColorInformation) or a thenable that resolves to such. The lack of a result
can be signaled by returning `undefined`, `null`, or an empty array.
