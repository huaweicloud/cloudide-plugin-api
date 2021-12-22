**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TypeDefinitionProvider

# Interface: TypeDefinitionProvider

The type definition provider defines the contract between extensions and
the go to type definition feature.

## Hierarchy

* **TypeDefinitionProvider**

## Index

### Methods

* [provideTypeDefinition](_index_d_._plugin_.typedefinitionprovider.md#providetypedefinition)

## Methods

### provideTypeDefinition

▸ **provideTypeDefinition**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Definition](../modules/_index_d_._plugin_.md#definition) \| [DefinitionLink](../modules/_index_d_._plugin_.md#definitionlink)[]>

*Defined in [index.d.ts:2603](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2603)*

Provide the type definition of the symbol at the given position and document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Definition](../modules/_index_d_._plugin_.md#definition) \| [DefinitionLink](../modules/_index_d_._plugin_.md#definitionlink)[]>

A definition or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.
