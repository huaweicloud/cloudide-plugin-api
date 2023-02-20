**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / EvaluatableExpressionProvider

# Interface: EvaluatableExpressionProvider

The evaluatable expression provider interface defines the contract between extensions and
the debug hover. In this contract the provider returns an evaluatable expression for a given position
in a document and VS Code evaluates this expression in the active debug session and shows the result in a debug hover.

## Hierarchy

* **EvaluatableExpressionProvider**

## Index

### Methods

* [provideEvaluatableExpression](_index_d_._plugin_.evaluatableexpressionprovider.md#provideevaluatableexpression)

## Methods

### provideEvaluatableExpression

▸ **provideEvaluatableExpression**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[EvaluatableExpression](../classes/_index_d_._plugin_.evaluatableexpression.md)>

*Defined in [index.d.ts:2785](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L2785)*

Provide an evaluatable expression for the given document and position.
VS Code will evaluate this expression in the active debug session and will show the result in the debug hover.
The expression can be implicitly specified by the range in the underlying document or by explicitly returning an expression.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document for which the debug hover is about to appear. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The line and character position in the document where the debug hover is about to appear. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[EvaluatableExpression](../classes/_index_d_._plugin_.evaluatableexpression.md)>

An EvaluatableExpression or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.
