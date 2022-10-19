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

[index.d.ts:5498](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5498)

___

### indentAction

• **indentAction**: [`IndentAction`](../enums/codearts_plugin_.IndentAction.md)

Describe what to do with the indentation.

#### Defined in

[index.d.ts:5494](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5494)

___

### removeText

• `Optional` **removeText**: `number`

Describes the number of characters to remove from the new line's indentation.

#### Defined in

[index.d.ts:5502](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5502)
