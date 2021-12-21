**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / IndentationRule

# Interface: IndentationRule

Describes indentation rules for a language.

## Hierarchy

* **IndentationRule**

## Index

### Properties

* [decreaseIndentPattern](_index_d_._plugin_.indentationrule.md#decreaseindentpattern)
* [increaseIndentPattern](_index_d_._plugin_.indentationrule.md#increaseindentpattern)
* [indentNextLinePattern](_index_d_._plugin_.indentationrule.md#indentnextlinepattern)
* [unIndentedLinePattern](_index_d_._plugin_.indentationrule.md#unindentedlinepattern)

## Properties

### decreaseIndentPattern

•  **decreaseIndentPattern**: RegExp

*Defined in [index.d.ts:4749](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4749)*

If a line matches this pattern, then all the lines after it should be unindented once (until another rule matches).

___

### increaseIndentPattern

•  **increaseIndentPattern**: RegExp

*Defined in [index.d.ts:4753](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4753)*

If a line matches this pattern, then all the lines after it should be indented once (until another rule matches).

___

### indentNextLinePattern

• `Optional` **indentNextLinePattern**: RegExp

*Defined in [index.d.ts:4757](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4757)*

If a line matches this pattern, then **only the next line** after it should be indented once.

___

### unIndentedLinePattern

• `Optional` **unIndentedLinePattern**: RegExp

*Defined in [index.d.ts:4761](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4761)*

If a line matches this pattern, then its indentation should not be changed and it should not be evaluated against the other rules.
