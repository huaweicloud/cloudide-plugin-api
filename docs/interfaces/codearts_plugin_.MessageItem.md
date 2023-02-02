[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / MessageItem

# Interface: MessageItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).MessageItem

Represents an action that is shown with an information, warning, or
error message.

**`See`**

 - [showInformationMessage](../modules/codearts_plugin_.window.md#showinformationmessage)
 - [showWarningMessage](../modules/codearts_plugin_.window.md#showwarningmessage)
 - [showErrorMessage](../modules/codearts_plugin_.window.md#showerrormessage)

## Table of contents

### Properties

- [isCloseAffordance](codearts_plugin_.MessageItem.md#iscloseaffordance)
- [title](codearts_plugin_.MessageItem.md#title)

## Properties

### isCloseAffordance

• `Optional` **isCloseAffordance**: `boolean`

A hint for modal dialogs that the item should be triggered
when the user cancels the dialog (e.g. by pressing the ESC
key).

Note: this option is ignored for non-modal messages.

#### Defined in

[index.d.ts:1962](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1962)

___

### title

• **title**: `string`

A short title like 'Retry', 'Open Log' etc.

#### Defined in

[index.d.ts:1953](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1953)
