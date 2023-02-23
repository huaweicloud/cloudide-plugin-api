[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / IndentationRule

# Interface: IndentationRule

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).IndentationRule

Describes indentation rules for a language.

## Table of contents

### Properties

- [decreaseIndentPattern](cloudide_plugin_.IndentationRule.md#decreaseindentpattern)
- [increaseIndentPattern](cloudide_plugin_.IndentationRule.md#increaseindentpattern)
- [indentNextLinePattern](cloudide_plugin_.IndentationRule.md#indentnextlinepattern)
- [unIndentedLinePattern](cloudide_plugin_.IndentationRule.md#unindentedlinepattern)

## Properties

### decreaseIndentPattern

• **decreaseIndentPattern**: `RegExp`

If a line matches this pattern, then all the lines after it should be unindented once (until another rule matches).

#### Defined in

[index.d.ts:6668](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6668)

___

### increaseIndentPattern

• **increaseIndentPattern**: `RegExp`

If a line matches this pattern, then all the lines after it should be indented once (until another rule matches).

#### Defined in

[index.d.ts:6672](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6672)

___

### indentNextLinePattern

• `Optional` **indentNextLinePattern**: `RegExp`

If a line matches this pattern, then **only the next line** after it should be indented once.

#### Defined in

[index.d.ts:6676](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6676)

___

### unIndentedLinePattern

• `Optional` **unIndentedLinePattern**: `RegExp`

If a line matches this pattern, then its indentation should not be changed and it should not be evaluated against the other rules.

#### Defined in

[index.d.ts:6680](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6680)
