**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / [window](../modules/_index_d_._plugin_.window.md) / CustomizableDialog

# Interface: CustomizableDialog

Represents the interface returned after a customizable dialog is created.

## Hierarchy

* **CustomizableDialog**

## Index

### Properties

* [data](_index_d_._plugin_.window.customizabledialog.md#data)
* [id](_index_d_._plugin_.window.customizabledialog.md#id)

### Methods

* [close](_index_d_._plugin_.window.customizabledialog.md#close)
* [updateButtons](_index_d_._plugin_.window.customizabledialog.md#updatebuttons)
* [updateContent](_index_d_._plugin_.window.customizabledialog.md#updatecontent)

## Properties

### data

•  **data**: string \| undefined

*Defined in [index.d.ts:8744](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8744)*

Data from the dialog.

___

### id

•  **id**: string

*Defined in [index.d.ts:8740](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8740)*

ID of iframe in the dialog.

## Methods

### close

▸ **close**(): void

*Defined in [index.d.ts:8736](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8736)*

Close the current dialog.

**Returns:** void

___

### updateButtons

▸ **updateButtons**(`buttons`: [DialogButton](_index_d_._plugin_.window.dialogbutton.md)[]): void

*Defined in [index.d.ts:8752](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8752)*

Update the buttons of the current dialog.

#### Parameters:

Name | Type |
------ | ------ |
`buttons` | [DialogButton](_index_d_._plugin_.window.dialogbutton.md)[] |

**Returns:** void

___

### updateContent

▸ **updateContent**(`content`: string): void

*Defined in [index.d.ts:8748](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8748)*

Update the content of the current dialog.

#### Parameters:

Name | Type |
------ | ------ |
`content` | string |

**Returns:** void
