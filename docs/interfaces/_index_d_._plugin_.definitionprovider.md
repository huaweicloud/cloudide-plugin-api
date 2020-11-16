**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DefinitionProvider

# Interface: DefinitionProvider

The definition provider interface defines the contract between extensions and
the [go to definition](https://code.visualstudio.com/docs/editor/editingevolved#_go-to-definition)
and peek definition features.

## Hierarchy

* **DefinitionProvider**

## Index

### Methods

* [provideDefinition](_index_d_._plugin_.definitionprovider.md#providedefinition)

## Methods

### provideDefinition

▸ **provideDefinition**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Definition](../modules/_index_d_._plugin_.md#definition) \| [DefinitionLink](../modules/_index_d_._plugin_.md#definitionlink)[]>

*Defined in [index.d.ts:2342](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2342)*

Provide the definition of the symbol at the given position and document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Definition](../modules/_index_d_._plugin_.md#definition) \| [DefinitionLink](../modules/_index_d_._plugin_.md#definitionlink)[]>

A definition or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.
