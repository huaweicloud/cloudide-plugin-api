[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / [ui](../modules/codearts_plugin_.ui.md) / ActionViewItem

# Interface: ActionViewItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).[ui](../modules/codearts_plugin_.ui.md).ActionViewItem

ActionViewItem Control.

## Hierarchy

- [`Component`](codearts_plugin_.ui.Component.md)

  ↳ **`ActionViewItem`**

## Table of contents

### Properties

- [action](codearts_plugin_.ui.ActionViewItem-1.md#action)
- [id](codearts_plugin_.ui.ActionViewItem-1.md#id)
- [ideuiModule](codearts_plugin_.ui.ActionViewItem-1.md#ideuimodule)
- [onClick](codearts_plugin_.ui.ActionViewItem-1.md#onclick)
- [onConnected](codearts_plugin_.ui.ActionViewItem-1.md#onconnected)
- [onDisconnected](codearts_plugin_.ui.ActionViewItem-1.md#ondisconnected)
- [options](codearts_plugin_.ui.ActionViewItem-1.md#options)

### Methods

- [blur](codearts_plugin_.ui.ActionViewItem-1.md#blur)
- [dispose](codearts_plugin_.ui.ActionViewItem-1.md#dispose)
- [focus](codearts_plugin_.ui.ActionViewItem-1.md#focus)
- [isFocused](codearts_plugin_.ui.ActionViewItem-1.md#isfocused)
- [on](codearts_plugin_.ui.ActionViewItem-1.md#on)
- [order](codearts_plugin_.ui.ActionViewItem-1.md#order)
- [render](codearts_plugin_.ui.ActionViewItem-1.md#render)
- [setFocusable](codearts_plugin_.ui.ActionViewItem-1.md#setfocusable)
- [updateClass](codearts_plugin_.ui.ActionViewItem-1.md#updateclass)
- [updateLabel](codearts_plugin_.ui.ActionViewItem-1.md#updatelabel)
- [updateTooltip](codearts_plugin_.ui.ActionViewItem-1.md#updatetooltip)

## Properties

### action

• **action**: [`ActionOptions`](codearts_plugin_.ui.ActionOptions.md)

Action parameters.

#### Defined in

[index.d.ts:17310](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17310)

___

### id

• **id**: `string`

The unique id of ActionViewItem control.

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[id](codearts_plugin_.ui.Component.md#id)

#### Defined in

[index.d.ts:17305](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17305)

___

### ideuiModule

• **ideuiModule**: `string`

The frontend module name corresponding to this control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[ideuiModule](codearts_plugin_.ui.Component.md#ideuimodule)

#### Defined in

[index.d.ts:17204](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17204)

___

### onClick

• **onClick**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Callback when a ActionViewItem is clicked.

#### Defined in

[index.d.ts:17320](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17320)

___

### onConnected

• **onConnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is mounted in front-end dom.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[onConnected](codearts_plugin_.ui.Component.md#onconnected)

#### Defined in

[index.d.ts:17214](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17214)

___

### onDisconnected

• **onDisconnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is unmounted in front-end dom.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[onDisconnected](codearts_plugin_.ui.Component.md#ondisconnected)

#### Defined in

[index.d.ts:17219](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17219)

___

### options

• **options**: [`ActionViewItemOptions`](codearts_plugin_.ui.ActionViewItemOptions.md)

Configuration parameters of the ActionViewItem component.

#### Defined in

[index.d.ts:17315](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17315)

## Methods

### blur

▸ **blur**(): `void`

Blur the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17340](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17340)

___

### dispose

▸ **dispose**(): `void`

Destroy the component.

#### Returns

`void`

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[dispose](codearts_plugin_.ui.Component.md#dispose)

#### Defined in

[index.d.ts:17365](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17365)

___

### focus

▸ **focus**(): `void`

Focus the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17330](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17330)

___

### isFocused

▸ **isFocused**(): `boolean`

Determine whether the current element is focused.

#### Returns

`boolean`

#### Defined in

[index.d.ts:17335](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17335)

___

### on

▸ **on**(`eventType`, `eventhandler`): `void`

Listen for events, the `eventType` here can only support the event type that the control encapsulates in the `mainthread`.

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventType` | `string` |
| `eventhandler` | (`eventData`: `any`) => `void` |

#### Returns

`void`

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[on](codearts_plugin_.ui.Component.md#on)

#### Defined in

[index.d.ts:17224](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17224)

___

### order

▸ **order**(): `number`

Obtains the order of the current component.

#### Returns

`number`

#### Defined in

[index.d.ts:17370](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17370)

___

### render

▸ **render**(): `void`

Render an html element from the action view item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17325](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17325)

___

### setFocusable

▸ **setFocusable**(): `void`

Event for modifying item focusable when dot is set.

#### Returns

`void`

#### Defined in

[index.d.ts:17345](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17345)

___

### updateClass

▸ **updateClass**(): `void`

Update the class of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17350](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17350)

___

### updateLabel

▸ **updateLabel**(): `void`

Update the label of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17355](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17355)

___

### updateTooltip

▸ **updateTooltip**(): `void`

Update the tooltip of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17360](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17360)
