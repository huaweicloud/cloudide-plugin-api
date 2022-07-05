[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / EvaluatableExpressionProvider

# Interface: EvaluatableExpressionProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).EvaluatableExpressionProvider

## Table of contents

### Methods

- [provideEvaluatableExpression](codearts_plugin_.EvaluatableExpressionProvider.md#provideevaluatableexpression)

## Methods

### provideEvaluatableExpression

▸ **provideEvaluatableExpression**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`EvaluatableExpression`](../classes/codearts_plugin_.EvaluatableExpression.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`EvaluatableExpression`](../classes/codearts_plugin_.EvaluatableExpression.md)\>

#### Defined in

[index.d.ts:2923](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L2923)
