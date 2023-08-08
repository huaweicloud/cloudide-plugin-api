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

[index.d.ts:17523](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17523)

___

### id

• **id**: `string`

The unique id of ActionViewItem control.

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[id](codearts_plugin_.ui.Component.md#id)

#### Defined in

[index.d.ts:17518](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17518)

___

### ideuiModule

• **ideuiModule**: `string`

The frontend module name corresponding to this control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[ideuiModule](codearts_plugin_.ui.Component.md#ideuimodule)

#### Defined in

[index.d.ts:17417](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17417)

___

### onClick

• **onClick**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Callback when a ActionViewItem is clicked.

#### Defined in

[index.d.ts:17533](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17533)

___

### onConnected

• **onConnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is mounted in front-end dom.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[onConnected](codearts_plugin_.ui.Component.md#onconnected)

#### Defined in

[index.d.ts:17427](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17427)

___

### onDisconnected

• **onDisconnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is unmounted in front-end dom.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[onDisconnected](codearts_plugin_.ui.Component.md#ondisconnected)

#### Defined in

[index.d.ts:17432](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17432)

___

### options

• **options**: [`ActionViewItemOptions`](codearts_plugin_.ui.ActionViewItemOptions.md)

Configuration parameters of the ActionViewItem component.

#### Defined in

[index.d.ts:17528](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17528)

## Methods

### blur

▸ **blur**(): `void`

Blur the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17553](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17553)

___

### dispose

▸ **dispose**(): `void`

Destroy the component.

#### Returns

`void`

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[dispose](codearts_plugin_.ui.Component.md#dispose)

#### Defined in

[index.d.ts:17578](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17578)

___

### focus

▸ **focus**(): `void`

Focus the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17543](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17543)

___

### isFocused

▸ **isFocused**(): `boolean`

Determine whether the current element is focused.

#### Returns

`boolean`

#### Defined in

[index.d.ts:17548](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17548)

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

[index.d.ts:17437](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17437)

___

### order

▸ **order**(): `number`

Obtains the order of the current component.

#### Returns

`number`

#### Defined in

[index.d.ts:17583](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17583)

___

### render

▸ **render**(): `void`

Render an html element from the action view item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17538](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17538)

___

### setFocusable

▸ **setFocusable**(): `void`

Event for modifying item focusable when dot is set.

#### Returns

`void`

#### Defined in

[index.d.ts:17558](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17558)

___

### updateClass

▸ **updateClass**(): `void`

Update the class of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17563](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17563)

___

### updateLabel

▸ **updateLabel**(): `void`

Update the label of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17568](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17568)

___

### updateTooltip

▸ **updateTooltip**(): `void`

Update the tooltip of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17573](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17573)
