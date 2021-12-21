**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / MessageItem

# Interface: MessageItem

Represents an action that is shown with an information, warning, or
error message.

**`see`** [showInformationMessage](#window.showInformationMessage)

**`see`** [showWarningMessage](#window.showWarningMessage)

**`see`** [showErrorMessage](#window.showErrorMessage)

## Hierarchy

* **MessageItem**

## Index

### Properties

* [isCloseAffordance](_index_d_._plugin_.messageitem.md#iscloseaffordance)
* [title](_index_d_._plugin_.messageitem.md#title)

## Properties

### isCloseAffordance

• `Optional` **isCloseAffordance**: boolean

*Defined in [index.d.ts:1945](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1945)*

A hint for modal dialogs that the item should be triggered
when the user cancels the dialog (e.g. by pressing the ESC
key).

Note: this option is ignored for non-modal messages.

___

### title

•  **title**: string

*Defined in [index.d.ts:1936](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1936)*

A short title like 'Retry', 'Open Log' etc.
