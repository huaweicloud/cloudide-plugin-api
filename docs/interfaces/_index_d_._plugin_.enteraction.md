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

*Defined in [index.d.ts:4799](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4799)*

Describes text to be appended after the new line and after the indentation.

___

### indentAction

•  **indentAction**: [IndentAction](../enums/_index_d_._plugin_.indentaction.md)

*Defined in [index.d.ts:4795](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4795)*

Describe what to do with the indentation.

___

### removeText

• `Optional` **removeText**: number

*Defined in [index.d.ts:4803](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4803)*

Describes the number of characters to remove from the new line's indentation.
