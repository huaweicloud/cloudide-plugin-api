[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / [window](../modules/cloudide_plugin_.window.md) / CustomizableDialog

# Interface: CustomizableDialog

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).[window](../modules/cloudide_plugin_.window.md).CustomizableDialog

Represents the interface returned after a customizable dialog is created.

## Table of contents

### Properties

- [data](cloudide_plugin_.window.CustomizableDialog.md#data)
- [id](cloudide_plugin_.window.CustomizableDialog.md#id)

### Methods

- [close](cloudide_plugin_.window.CustomizableDialog.md#close)
- [updateButtons](cloudide_plugin_.window.CustomizableDialog.md#updatebuttons)
- [updateContent](cloudide_plugin_.window.CustomizableDialog.md#updatecontent)

## Properties

### data

• **data**: `undefined` \| `string`

Data from the dialog.

#### Defined in

[index.d.ts:4533](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4533)

___

### id

• **id**: `string`

ID of iframe in the dialog.

#### Defined in

[index.d.ts:4529](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4529)

## Methods

### close

▸ **close**(): `void`

Close the current dialog.

#### Returns

`void`

#### Defined in

[index.d.ts:4525](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4525)

___

### updateButtons

▸ **updateButtons**(`buttons`): `void`

Update the buttons of the current dialog.

#### Parameters

| Name | Type |
| :------ | :------ |
| `buttons` | [`DialogButton`](cloudide_plugin_.window.DialogButton.md)[] |

#### Returns

`void`

#### Defined in

[index.d.ts:4541](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4541)

___

### updateContent

▸ **updateContent**(`content`): `void`

Update the content of the current dialog.

#### Parameters

| Name | Type |
| :------ | :------ |
| `content` | `string` |

#### Returns

`void`

#### Defined in

[index.d.ts:4537](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4537)
