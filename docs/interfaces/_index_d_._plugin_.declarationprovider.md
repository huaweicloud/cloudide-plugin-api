**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DeclarationProvider

# Interface: DeclarationProvider

The declaration provider interface defines the contract between extensions and
the go to declaration feature.

## Hierarchy

* **DeclarationProvider**

## Index

### Methods

* [provideDeclaration](_index_d_._plugin_.declarationprovider.md#providedeclaration)

## Methods

### provideDeclaration

▸ **provideDeclaration**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Declaration](../modules/_index_d_._plugin_.md#declaration)>

*Defined in [index.d.ts:2624](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2624)*

Provide the declaration of the symbol at the given position and document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Declaration](../modules/_index_d_._plugin_.md#declaration)>

A declaration or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.
