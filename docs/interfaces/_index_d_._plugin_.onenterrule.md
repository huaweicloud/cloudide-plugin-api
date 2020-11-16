**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / OnEnterRule

# Interface: OnEnterRule

Describes a rule to be evaluated when pressing Enter.

## Hierarchy

* **OnEnterRule**

## Index

### Properties

* [action](_index_d_._plugin_.onenterrule.md#action)
* [afterText](_index_d_._plugin_.onenterrule.md#aftertext)
* [beforeText](_index_d_._plugin_.onenterrule.md#beforetext)

## Properties

### action

•  **action**: [EnterAction](_index_d_._plugin_.enteraction.md)

*Defined in [index.d.ts:4531](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4531)*

The action to execute.

___

### afterText

• `Optional` **afterText**: RegExp

*Defined in [index.d.ts:4527](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4527)*

This rule will only execute if the text after the cursor matches this regular expression.

___

### beforeText

•  **beforeText**: RegExp

*Defined in [index.d.ts:4523](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4523)*

This rule will only execute if the text before the cursor matches this regular expression.
