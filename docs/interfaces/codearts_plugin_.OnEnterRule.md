[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / OnEnterRule

# Interface: OnEnterRule

["@codearts/plugin"](../modules/_codearts_plugin_.md).OnEnterRule

Describes a rule to be evaluated when pressing Enter.

## Table of contents

### Properties

- [action](codearts_plugin_.OnEnterRule.md#action)
- [afterText](codearts_plugin_.OnEnterRule.md#aftertext)
- [beforeText](codearts_plugin_.OnEnterRule.md#beforetext)
- [previousLineText](codearts_plugin_.OnEnterRule.md#previouslinetext)

## Properties

### action

• **action**: [`EnterAction`](codearts_plugin_.EnterAction.md)

The action to execute.

#### Defined in

[index.d.ts:5595](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5595)

___

### afterText

• `Optional` **afterText**: `RegExp`

This rule will only execute if the text after the cursor matches this regular expression.

#### Defined in

[index.d.ts:5587](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5587)

___

### beforeText

• **beforeText**: `RegExp`

This rule will only execute if the text before the cursor matches this regular expression.

#### Defined in

[index.d.ts:5583](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5583)

___

### previousLineText

• `Optional` **previousLineText**: `RegExp`

This rule will only execute if the text above the current line matches this regular expression.

#### Defined in

[index.d.ts:5591](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5591)
