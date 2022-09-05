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

[index.d.ts:5524](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5524)

___

### afterText

• `Optional` **afterText**: `RegExp`

This rule will only execute if the text after the cursor matches this regular expression.

#### Defined in

[index.d.ts:5516](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5516)

___

### beforeText

• **beforeText**: `RegExp`

This rule will only execute if the text before the cursor matches this regular expression.

#### Defined in

[index.d.ts:5512](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5512)

___

### previousLineText

• `Optional` **previousLineText**: `RegExp`

This rule will only execute if the text above the current line matches this regular expression.

#### Defined in

[index.d.ts:5520](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5520)
