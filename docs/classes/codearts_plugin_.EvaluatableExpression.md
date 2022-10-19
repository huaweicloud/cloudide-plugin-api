[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / EvaluatableExpression

# Class: EvaluatableExpression

["@codearts/plugin"](../modules/_codearts_plugin_.md).EvaluatableExpression

An EvaluatableExpression represents an expression in a document that can be evaluated by an active debugger or runtime.
The result of this evaluation is shown in a tooltip-like widget.
If only a range is specified, the expression will be extracted from the underlying document.
An optional expression can be used to override the extracted expression.
In this case the range is still used to highlight the range in the document.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.EvaluatableExpression.md#constructor)

### Properties

- [expression](codearts_plugin_.EvaluatableExpression.md#expression)
- [range](codearts_plugin_.EvaluatableExpression.md#range)

## Constructors

### constructor

• **new EvaluatableExpression**(`range`, `expression?`)

Creates a new evaluatable expression object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The range in the underlying document from which the evaluatable expression is extracted. |
| `expression?` | `string` | If specified overrides the extracted expression. |

#### Defined in

[index.d.ts:2902](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L2902)

## Properties

### expression

• `Optional` `Readonly` **expression**: `string`

#### Defined in

[index.d.ts:2894](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L2894)

___

### range

• `Readonly` **range**: [`Range`](codearts_plugin_.Range.md)

#### Defined in

[index.d.ts:2889](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L2889)
