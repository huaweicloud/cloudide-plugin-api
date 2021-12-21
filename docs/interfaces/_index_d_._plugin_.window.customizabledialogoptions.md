**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / [window](../modules/_index_d_._plugin_.window.md) / CustomizableDialogOptions

# Interface: CustomizableDialogOptions

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

*Defined in [index.d.ts:8665](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L8665)*

Buttons displayed at the bottom of the dialog box.

___

### buttonsAlign

• `Optional` **buttonsAlign**: \"left\" \| \"center\" \| \"right\"

*Defined in [index.d.ts:8669](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L8669)*

Button alignment mode. Default to be right.

___

### content

•  **content**: string

*Defined in [index.d.ts:8657](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L8657)*

HTML content or url nested in the iframe in the dialog box.

___

### disableCloseIcon

• `Optional` **disableCloseIcon**: boolean

*Defined in [index.d.ts:8661](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L8661)*

Whether to disable the close button in the upper right corner of the dialog box. Defaults to false.

___

### height

• `Optional` **height**: number

*Defined in [index.d.ts:8678](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L8678)*

Height of content in pixels.

___

### onClose

• `Optional` **onClose**: (event: [CustomizableDialogEvent](_index_d_._plugin_.window.customizabledialogevent.md)) => void

*Defined in [index.d.ts:8670](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L8670)*

___

### title

•  **title**: string

*Defined in [index.d.ts:8653](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L8653)*

Title displayed at the top of the dialog box.

___

### width

• `Optional` **width**: number

*Defined in [index.d.ts:8674](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L8674)*

Width of content in pixels.
