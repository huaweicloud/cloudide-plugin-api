**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / [window](../modules/_index_d_._plugin_.window.md) / CustomizableDialogOptions

# Interface: CustomizableDialogOptions

Represents options to create a customizable dialog.

## Hierarchy

* **CustomizableDialogOptions**

## Index

### Properties

* [buttons](_index_d_._plugin_.window.customizabledialogoptions.md#buttons)
* [buttonsAlign](_index_d_._plugin_.window.customizabledialogoptions.md#buttonsalign)
* [content](_index_d_._plugin_.window.customizabledialogoptions.md#content)
* [disableCloseIcon](_index_d_._plugin_.window.customizabledialogoptions.md#disablecloseicon)
* [height](_index_d_._plugin_.window.customizabledialogoptions.md#height)
* [onClose](_index_d_._plugin_.window.customizabledialogoptions.md#onclose)
* [title](_index_d_._plugin_.window.customizabledialogoptions.md#title)
* [width](_index_d_._plugin_.window.customizabledialogoptions.md#width)

## Properties

### buttons

• `Optional` **buttons**: [DialogButton](_index_d_._plugin_.window.dialogbutton.md)[]

*Defined in [index.d.ts:8672](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8672)*

Buttons displayed at the bottom of the dialog box.

___

### buttonsAlign

• `Optional` **buttonsAlign**: \"left\" \| \"center\" \| \"right\"

*Defined in [index.d.ts:8676](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8676)*

Button alignment mode. Default to be right.

___

### content

•  **content**: string

*Defined in [index.d.ts:8664](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8664)*

HTML content or url nested in the iframe in the dialog box.

___

### disableCloseIcon

• `Optional` **disableCloseIcon**: boolean

*Defined in [index.d.ts:8668](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8668)*

Whether to disable the close button in the upper right corner of the dialog box. Defaults to false.

___

### height

• `Optional` **height**: number

*Defined in [index.d.ts:8685](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8685)*

Height of content in pixels.

___

### onClose

• `Optional` **onClose**: (event: [CustomizableDialogEvent](_index_d_._plugin_.window.customizabledialogevent.md)) => void

*Defined in [index.d.ts:8677](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8677)*

___

### title

•  **title**: string

*Defined in [index.d.ts:8660](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8660)*

Title displayed at the top of the dialog box.

___

### width

• `Optional` **width**: number

*Defined in [index.d.ts:8681](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8681)*

Width of content in pixels.
