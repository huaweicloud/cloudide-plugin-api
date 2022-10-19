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

[index.d.ts:5448](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5448)

___

### increaseIndentPattern

• **increaseIndentPattern**: `RegExp`

If a line matches this pattern, then all the lines after it should be indented once (until another rule matches).

#### Defined in

[index.d.ts:5452](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5452)

___

### indentNextLinePattern

• `Optional` **indentNextLinePattern**: `RegExp`

If a line matches this pattern, then **only the next line** after it should be indented once.

#### Defined in

[index.d.ts:5456](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5456)

___

### unIndentedLinePattern

• `Optional` **unIndentedLinePattern**: `RegExp`

If a line matches this pattern, then its indentation should not be changed and it should not be evaluated against the other rules.

#### Defined in

[index.d.ts:5460](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5460)
