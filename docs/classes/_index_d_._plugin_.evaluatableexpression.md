**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / EvaluatableExpression

# Class: EvaluatableExpression

An EvaluatableExpression represents an expression in a document that can be evaluated by an active debugger or runtime.
The result of this evaluation is shown in a tooltip-like widget.
If only a range is specified, the expression will be extracted from the underlying document.
An optional expression can be used to override the extracted expression.
In this case the range is still used to highlight the range in the document.

## Hierarchy

* **EvaluatableExpression**

## Index

### Constructors

* [constructor](_index_d_._plugin_.evaluatableexpression.md#constructor)

### Properties

* [expression](_index_d_._plugin_.evaluatableexpression.md#expression)
* [range](_index_d_._plugin_.evaluatableexpression.md#range)

## Constructors

### constructor

\+ **new EvaluatableExpression**(`range`: [Range](_index_d_._plugin_.range.md), `expression?`: string): [EvaluatableExpression](_index_d_._plugin_.evaluatableexpression.md)

*Defined in [index.d.ts:2756](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L2756)*

Creates a new evaluatable expression object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | The range in the underlying document from which the evaluatable expression is extracted. |
`expression?` | string | If specified overrides the extracted expression.  |

**Returns:** [EvaluatableExpression](_index_d_._plugin_.evaluatableexpression.md)

## Properties

### expression

• `Optional` `Readonly` **expression**: string

*Defined in [index.d.ts:2756](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L2756)*

___

### range

• `Readonly` **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:2751](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L2751)*
