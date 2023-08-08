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

[index.d.ts:5582](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5582)

___

### afterText

• `Optional` **afterText**: `RegExp`

This rule will only execute if the text after the cursor matches this regular expression.

#### Defined in

[index.d.ts:5574](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5574)

___

### beforeText

• **beforeText**: `RegExp`

This rule will only execute if the text before the cursor matches this regular expression.

#### Defined in

[index.d.ts:5570](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5570)

___

### previousLineText

• `Optional` **previousLineText**: `RegExp`

This rule will only execute if the text above the current line matches this regular expression.

#### Defined in

[index.d.ts:5578](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5578)
