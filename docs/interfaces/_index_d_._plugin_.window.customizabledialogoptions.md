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

*Defined in [index.d.ts:8680](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8680)*

Buttons displayed at the bottom of the dialog.

___

### buttonsAlign

• `Optional` **buttonsAlign**: \"left\" \| \"center\" \| \"right\"

*Defined in [index.d.ts:8684](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8684)*

Button alignment mode. Default to be right.

___

### content

•  **content**: string

*Defined in [index.d.ts:8672](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8672)*

HTML content or url nested in the iframe in the dialog.

___

### disableCloseIcon

• `Optional` **disableCloseIcon**: boolean

*Defined in [index.d.ts:8676](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8676)*

Whether to disable the close button in the upper right corner of the dialog. Defaults to false.

___

### height

• `Optional` **height**: string

*Defined in [index.d.ts:8696](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8696)*

Height of content. *Note* that bring unit.

___

### onClose

• `Optional` **onClose**: (event: [CustomizableDialogEvent](_index_d_._plugin_.window.customizabledialogevent.md)) => void

*Defined in [index.d.ts:8688](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8688)*

Callback triggered when the dialog is closed.

___

### title

•  **title**: string

*Defined in [index.d.ts:8668](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8668)*

Title displayed at the top of the dialog.

___

### width

• `Optional` **width**: string

*Defined in [index.d.ts:8692](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8692)*

Width of content. *Note* that bring unit.
