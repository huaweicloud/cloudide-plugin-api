**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / HoverProvider

# Interface: HoverProvider

The hover provider interface defines the contract between extensions and
the [hover](https://code.visualstudio.com/docs/editor/intellisense)-feature.

## Hierarchy

* **HoverProvider**

## Index

### Methods

* [provideHover](_index_d_._plugin_.hoverprovider.md#providehover)

## Methods

### provideHover

▸ **provideHover**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Hover](../classes/_index_d_._plugin_.hover.md)>

*Defined in [index.d.ts:2736](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L2736)*

Provide a hover for the given position and document. Multiple hovers at the same
position will be merged by the editor. A hover can have a range which defaults
to the word range at the position when omitted.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Hover](../classes/_index_d_._plugin_.hover.md)>

A hover or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.
