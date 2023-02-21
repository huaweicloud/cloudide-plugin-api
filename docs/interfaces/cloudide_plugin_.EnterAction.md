[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / EnterAction

# Interface: EnterAction

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).EnterAction

Describes what to do when pressing Enter.

## Table of contents

### Properties

- [appendText](cloudide_plugin_.EnterAction.md#appendtext)
- [indentAction](cloudide_plugin_.EnterAction.md#indentaction)
- [removeText](cloudide_plugin_.EnterAction.md#removetext)

## Properties

### appendText

• `Optional` **appendText**: `string`

Describes text to be appended after the new line and after the indentation.

#### Defined in

[index.d.ts:6636](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6636)

___

### indentAction

• **indentAction**: [`IndentAction`](../enums/cloudide_plugin_.IndentAction.md)

Describe what to do with the indentation.

#### Defined in

[index.d.ts:6632](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6632)

___

### removeText

• `Optional` **removeText**: `number`

Describes the number of characters to remove from the new line's indentation.

#### Defined in

[index.d.ts:6640](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6640)
