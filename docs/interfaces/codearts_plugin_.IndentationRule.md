[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / IndentationRule

# Interface: IndentationRule

["@codearts/plugin"](../modules/_codearts_plugin_.md).IndentationRule

Describes indentation rules for a language.

## Table of contents

### Properties

- [decreaseIndentPattern](codearts_plugin_.IndentationRule.md#decreaseindentpattern)
- [increaseIndentPattern](codearts_plugin_.IndentationRule.md#increaseindentpattern)
- [indentNextLinePattern](codearts_plugin_.IndentationRule.md#indentnextlinepattern)
- [unIndentedLinePattern](codearts_plugin_.IndentationRule.md#unindentedlinepattern)

## Properties

### decreaseIndentPattern

• **decreaseIndentPattern**: `RegExp`

If a line matches this pattern, then all the lines after it should be unindented once (until another rule matches).

#### Defined in

[index.d.ts:5468](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5468)

___

### increaseIndentPattern

• **increaseIndentPattern**: `RegExp`

If a line matches this pattern, then all the lines after it should be indented once (until another rule matches).

#### Defined in

[index.d.ts:5472](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5472)

___

### indentNextLinePattern

• `Optional` **indentNextLinePattern**: `RegExp`

If a line matches this pattern, then **only the next line** after it should be indented once.

#### Defined in

[index.d.ts:5476](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5476)

___

### unIndentedLinePattern

• `Optional` **unIndentedLinePattern**: `RegExp`

If a line matches this pattern, then its indentation should not be changed and it should not be evaluated against the other rules.

#### Defined in

[index.d.ts:5480](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5480)
