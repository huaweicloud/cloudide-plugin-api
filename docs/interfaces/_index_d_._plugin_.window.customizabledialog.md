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

*Defined in [index.d.ts:8730](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8730)*

Data from the dialog box.

___

### id

•  **id**: string

*Defined in [index.d.ts:8726](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8726)*

ID of iframe in the dialog box.

## Methods

### close

▸ **close**(): void

*Defined in [index.d.ts:8722](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8722)*

Close the current dialog box.

**Returns:** void

___

### updateButtons

▸ **updateButtons**(`buttons`: [DialogButton](_index_d_._plugin_.window.dialogbutton.md)[]): void

*Defined in [index.d.ts:8738](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8738)*

Update the buttons of the current dialog box.

#### Parameters:

Name | Type |
------ | ------ |
`buttons` | [DialogButton](_index_d_._plugin_.window.dialogbutton.md)[] |

**Returns:** void

___

### updateContent

▸ **updateContent**(`content`: string): void

*Defined in [index.d.ts:8734](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8734)*

Update the content of the current dialog box.

#### Parameters:

Name | Type |
------ | ------ |
`content` | string |

**Returns:** void
