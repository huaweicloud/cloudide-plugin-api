[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / EvaluatableExpressionProvider

# Interface: EvaluatableExpressionProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).EvaluatableExpressionProvider

The evaluatable expression provider interface defines the contract between extensions and
the debug hover. In this contract the provider returns an evaluatable expression for a given position
in a document and the editor evaluates this expression in the active debug session and shows the result in a debug hover.

## Table of contents

### Methods

- [provideEvaluatableExpression](codearts_plugin_.EvaluatableExpressionProvider.md#provideevaluatableexpression)

## Methods

### provideEvaluatableExpression

▸ **provideEvaluatableExpression**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`EvaluatableExpression`](../classes/codearts_plugin_.EvaluatableExpression.md)\>

Provide an evaluatable expression for the given document and position.
The editor will evaluate this expression in the active debug session and will show the result in the debug hover.
The expression can be implicitly specified by the range in the underlying document or by explicitly returning an expression.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document for which the debug hover is about to appear. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The line and character position in the document where the debug hover is about to appear. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`EvaluatableExpression`](../classes/codearts_plugin_.EvaluatableExpression.md)\>

An EvaluatableExpression or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:2923](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2923)
