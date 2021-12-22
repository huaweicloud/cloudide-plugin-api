**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / QuickDiffProvider

# Interface: QuickDiffProvider

## Hierarchy

* **QuickDiffProvider**

## Index

### Methods

* [provideOriginalResource](_index_d_._plugin_.quickdiffprovider.md#provideoriginalresource)

## Methods

### provideOriginalResource

▸ `Optional`**provideOriginalResource**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Uri](../classes/_index_d_._plugin_.uri.md)>

*Defined in [index.d.ts:11270](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11270)*

Provide a [uri](#Uri) to the original resource of any given resource uri.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the resource open in a text editor. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Uri](../classes/_index_d_._plugin_.uri.md)>

A thenable that resolves to uri of the matching original resource.
