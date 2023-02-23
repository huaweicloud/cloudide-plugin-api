[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / [window](../modules/cloudide_plugin_.window.md) / CustomizableDialogOptions

# Interface: CustomizableDialogOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).[window](../modules/cloudide_plugin_.window.md).CustomizableDialogOptions

Represents options to create a customizable dialog.

## Table of contents

### Properties

- [buttons](cloudide_plugin_.window.CustomizableDialogOptions.md#buttons)
- [buttonsAlign](cloudide_plugin_.window.CustomizableDialogOptions.md#buttonsalign)
- [content](cloudide_plugin_.window.CustomizableDialogOptions.md#content)
- [disableCloseIcon](cloudide_plugin_.window.CustomizableDialogOptions.md#disablecloseicon)
- [height](cloudide_plugin_.window.CustomizableDialogOptions.md#height)
- [onClose](cloudide_plugin_.window.CustomizableDialogOptions.md#onclose)
- [title](cloudide_plugin_.window.CustomizableDialogOptions.md#title)
- [width](cloudide_plugin_.window.CustomizableDialogOptions.md#width)

## Properties

### buttons

• `Optional` **buttons**: [`DialogButton`](cloudide_plugin_.window.DialogButton.md)[]

Buttons displayed at the bottom of the dialog.

#### Defined in

[index.d.ts:4469](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4469)

___

### buttonsAlign

• `Optional` **buttonsAlign**: ``"left"`` \| ``"center"`` \| ``"right"``

Button alignment mode. Default to be right.

#### Defined in

[index.d.ts:4473](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4473)

___

### content

• **content**: `string`

HTML content or url nested in the iframe in the dialog.

#### Defined in

[index.d.ts:4461](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4461)

___

### disableCloseIcon

• `Optional` **disableCloseIcon**: `boolean`

Whether to disable the close button in the upper right corner of the dialog. Defaults to false.

#### Defined in

[index.d.ts:4465](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4465)

___

### height

• `Optional` **height**: `string`

Height of content. *Note* that bring unit.

#### Defined in

[index.d.ts:4485](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4485)

___

### onClose

• `Optional` **onClose**: (`event`: [`CustomizableDialogEvent`](cloudide_plugin_.window.CustomizableDialogEvent.md)) => `void`

#### Type declaration

▸ (`event`): `void`

Callback triggered when the dialog is closed.

##### Parameters

| Name | Type |
| :------ | :------ |
| `event` | [`CustomizableDialogEvent`](cloudide_plugin_.window.CustomizableDialogEvent.md) |

##### Returns

`void`

#### Defined in

[index.d.ts:4477](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4477)

___

### title

• **title**: `string`

Title displayed at the top of the dialog.

#### Defined in

[index.d.ts:4457](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4457)

___

### width

• `Optional` **width**: `string`

Width of content. *Note* that bring unit.

#### Defined in

[index.d.ts:4481](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4481)
