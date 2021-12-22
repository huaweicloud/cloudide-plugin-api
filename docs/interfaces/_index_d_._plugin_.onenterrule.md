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
* [previousLineText](_index_d_._plugin_.onenterrule.md#previouslinetext)

## Properties

### action

•  **action**: [EnterAction](_index_d_._plugin_.enteraction.md)

*Defined in [index.d.ts:4828](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4828)*

The action to execute.

___

### afterText

• `Optional` **afterText**: RegExp

*Defined in [index.d.ts:4820](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4820)*

This rule will only execute if the text after the cursor matches this regular expression.

___

### beforeText

•  **beforeText**: RegExp

*Defined in [index.d.ts:4816](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4816)*

This rule will only execute if the text before the cursor matches this regular expression.

___

### previousLineText

• `Optional` **previousLineText**: RegExp

*Defined in [index.d.ts:4824](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4824)*

This rule will only execute if the text above the current line matches this regular expression.
