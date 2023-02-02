[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / MessageOptions

# Interface: MessageOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).MessageOptions

Options to configure the behavior of the message.

**`See`**

 - [showInformationMessage](../modules/codearts_plugin_.window.md#showinformationmessage)
 - [showWarningMessage](../modules/codearts_plugin_.window.md#showwarningmessage)
 - [showErrorMessage](../modules/codearts_plugin_.window.md#showerrormessage)

## Table of contents

### Properties

- [detail](codearts_plugin_.MessageOptions.md#detail)
- [modal](codearts_plugin_.MessageOptions.md#modal)

## Properties

### detail

• `Optional` **detail**: `string`

Human-readable detail message that is rendered less prominent. _Note_ that detail
is only shown for [modal](codearts_plugin_.MessageOptions.md#modal) messages.

#### Defined in

[index.d.ts:1983](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1983)

___

### modal

• `Optional` **modal**: `boolean`

Indicates that this message should be modal.

#### Defined in

[index.d.ts:1977](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1977)
