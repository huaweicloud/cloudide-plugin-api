[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / [window](../modules/cloudide_plugin_.window.md) / CustomizableDialogEvent

# Interface: CustomizableDialogEvent

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).[window](../modules/cloudide_plugin_.window.md).CustomizableDialogEvent

Represents event of customizable,
used as the `onclose` callback parameter in `CustomizableDialogOptions`.

## Hierarchy

- [`Event`](cloudide_plugin_.Event.md)

  ↳ **`CustomizableDialogEvent`**

## Table of contents

### Properties

- [dialogData](cloudide_plugin_.window.CustomizableDialogEvent.md#dialogdata)
- [targetElement](cloudide_plugin_.window.CustomizableDialogEvent.md#targetelement)

## Properties

### dialogData

• `Optional` **dialogData**: `string`

Get cloudideDialogApis by `acquireCloudideDialogApi()`.
Call method `cloudideDialogApis.bindDialogData(data)` to emit data out, and get this data when dialog closed.

#### Defined in

[index.d.ts:4501](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4501)

___

### targetElement

• `Optional` **targetElement**: [`DialogControlElement`](cloudide_plugin_.window.DialogControlElement.md)

The target clicked when close the dialog.

#### Defined in

[index.d.ts:4496](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4496)
