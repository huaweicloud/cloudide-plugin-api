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

[index.d.ts:5506](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5506)

___

### increaseIndentPattern

• **increaseIndentPattern**: `RegExp`

If a line matches this pattern, then all the lines after it should be indented once (until another rule matches).

#### Defined in

[index.d.ts:5510](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5510)

___

### indentNextLinePattern

• `Optional` **indentNextLinePattern**: `RegExp`

If a line matches this pattern, then **only the next line** after it should be indented once.

#### Defined in

[index.d.ts:5514](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5514)

___

### unIndentedLinePattern

• `Optional` **unIndentedLinePattern**: `RegExp`

If a line matches this pattern, then its indentation should not be changed and it should not be evaluated against the other rules.

#### Defined in

[index.d.ts:5518](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5518)
