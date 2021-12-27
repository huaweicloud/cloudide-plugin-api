**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / EnterAction

# Interface: EnterAction

Describes what to do when pressing Enter.

## Hierarchy

* **EnterAction**

## Index

### Properties

* [appendText](_index_d_._plugin_.enteraction.md#appendtext)
* [indentAction](_index_d_._plugin_.enteraction.md#indentaction)
* [removeText](_index_d_._plugin_.enteraction.md#removetext)

## Properties

### appendText

• `Optional` **appendText**: string

*Defined in [index.d.ts:4802](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4802)*

Describes text to be appended after the new line and after the indentation.

___

### indentAction

•  **indentAction**: [IndentAction](../enums/_index_d_._plugin_.indentaction.md)

*Defined in [index.d.ts:4798](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4798)*

Describe what to do with the indentation.

___

### removeText

• `Optional` **removeText**: number

*Defined in [index.d.ts:4806](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4806)*

Describes the number of characters to remove from the new line's indentation.
