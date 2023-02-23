[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / OnEnterRule

# Interface: OnEnterRule

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).OnEnterRule

Describes a rule to be evaluated when pressing Enter.

## Table of contents

### Properties

- [action](cloudide_plugin_.OnEnterRule.md#action)
- [afterText](cloudide_plugin_.OnEnterRule.md#aftertext)
- [beforeText](cloudide_plugin_.OnEnterRule.md#beforetext)

## Properties

### action

• **action**: [`EnterAction`](cloudide_plugin_.EnterAction.md)

The action to execute.

#### Defined in

[index.d.ts:6658](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6658)

___

### afterText

• `Optional` **afterText**: `RegExp`

This rule will only execute if the text after the cursor matches this regular expression.

#### Defined in

[index.d.ts:6654](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6654)

___

### beforeText

• **beforeText**: `RegExp`

This rule will only execute if the text before the cursor matches this regular expression.

#### Defined in

[index.d.ts:6650](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6650)
