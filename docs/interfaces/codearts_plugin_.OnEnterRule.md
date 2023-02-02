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

[index.d.ts:5544](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5544)

___

### afterText

• `Optional` **afterText**: `RegExp`

This rule will only execute if the text after the cursor matches this regular expression.

#### Defined in

[index.d.ts:5536](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5536)

___

### beforeText

• **beforeText**: `RegExp`

This rule will only execute if the text before the cursor matches this regular expression.

#### Defined in

[index.d.ts:5532](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5532)

___

### previousLineText

• `Optional` **previousLineText**: `RegExp`

This rule will only execute if the text above the current line matches this regular expression.

#### Defined in

[index.d.ts:5540](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5540)
