[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineValueEvaluatableExpression

# Class: InlineValueEvaluatableExpression

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineValueEvaluatableExpression

Provide an inline value through an expression evaluation.
If only a range is specified, the expression will be extracted from the underlying document.
An optional expression can be used to override the extracted expression.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.InlineValueEvaluatableExpression.md#constructor)

### Properties

- [expression](codearts_plugin_.InlineValueEvaluatableExpression.md#expression)
- [range](codearts_plugin_.InlineValueEvaluatableExpression.md#range)

## Constructors

### constructor

• **new InlineValueEvaluatableExpression**(`range`, `expression?`)

Creates a new InlineValueEvaluatableExpression object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The range in the underlying document from which the evaluatable expression is extracted. |
| `expression?` | `string` | If specified overrides the extracted expression. |

#### Defined in

[index.d.ts:2997](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2997)

## Properties

### expression

• `Optional` `Readonly` **expression**: `string`

If specified the expression overrides the extracted expression.

#### Defined in

[index.d.ts:2990](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2990)

___

### range

• `Readonly` **range**: [`Range`](codearts_plugin_.Range.md)

The document range for which the inline value applies.
The range is used to extract the evaluatable expression from the underlying document.

#### Defined in

[index.d.ts:2986](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2986)
