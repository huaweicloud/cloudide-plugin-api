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

[index.d.ts:17507](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17507)

___

### id

• **id**: `string`

The unique id of ActionViewItem control.

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[id](codearts_plugin_.ui.Component.md#id)

#### Defined in

[index.d.ts:17502](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17502)

___

### ideuiModule

• **ideuiModule**: `string`

The frontend module name corresponding to this control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[ideuiModule](codearts_plugin_.ui.Component.md#ideuimodule)

#### Defined in

[index.d.ts:17401](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17401)

___

### onClick

• **onClick**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Callback when a ActionViewItem is clicked.

#### Defined in

[index.d.ts:17517](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17517)

___

### onConnected

• **onConnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is mounted in front-end dom.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[onConnected](codearts_plugin_.ui.Component.md#onconnected)

#### Defined in

[index.d.ts:17411](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17411)

___

### onDisconnected

• **onDisconnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is unmounted in front-end dom.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[onDisconnected](codearts_plugin_.ui.Component.md#ondisconnected)

#### Defined in

[index.d.ts:17416](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17416)

___

### options

• **options**: [`ActionViewItemOptions`](codearts_plugin_.ui.ActionViewItemOptions.md)

Configuration parameters of the ActionViewItem component.

#### Defined in

[index.d.ts:17512](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17512)

## Methods

### blur

▸ **blur**(): `void`

Blur the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17537](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17537)

___

### dispose

▸ **dispose**(): `void`

Destroy the component.

#### Returns

`void`

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[dispose](codearts_plugin_.ui.Component.md#dispose)

#### Defined in

[index.d.ts:17562](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17562)

___

### focus

▸ **focus**(): `void`

Focus the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17527](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17527)

___

### isFocused

▸ **isFocused**(): `boolean`

Determine whether the current element is focused.

#### Returns

`boolean`

#### Defined in

[index.d.ts:17532](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17532)

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

[index.d.ts:17421](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17421)

___

### order

▸ **order**(): `number`

Obtains the order of the current component.

#### Returns

`number`

#### Defined in

[index.d.ts:17567](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17567)

___

### render

▸ **render**(): `void`

Render an html element from the action view item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17522](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17522)

___

### setFocusable

▸ **setFocusable**(): `void`

Event for modifying item focusable when dot is set.

#### Returns

`void`

#### Defined in

[index.d.ts:17542](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17542)

___

### updateClass

▸ **updateClass**(): `void`

Update the class of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17547](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17547)

___

### updateLabel

▸ **updateLabel**(): `void`

Update the label of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17552](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17552)

___

### updateTooltip

▸ **updateTooltip**(): `void`

Update the tooltip of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17557](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17557)
