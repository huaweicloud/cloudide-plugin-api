[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / EnterAction

# Interface: EnterAction

["@codearts/plugin"](../modules/_codearts_plugin_.md).EnterAction

Describes what to do when pressing Enter.

## Table of contents

### Properties

- [appendText](codearts_plugin_.EnterAction.md#appendtext)
- [indentAction](codearts_plugin_.EnterAction.md#indentaction)
- [removeText](codearts_plugin_.EnterAction.md#removetext)

## Properties

### appendText

• `Optional` **appendText**: `string`

Describes text to be appended after the new line and after the indentation.

#### Defined in

[index.d.ts:5518](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5518)

___

### indentAction

• **indentAction**: [`IndentAction`](../enums/codearts_plugin_.IndentAction.md)

Describe what to do with the indentation.

#### Defined in

[index.d.ts:5514](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5514)

___

### removeText

• `Optional` **removeText**: `number`

Describes the number of characters to remove from the new line's indentation.

#### Defined in

[index.d.ts:5522](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5522)
