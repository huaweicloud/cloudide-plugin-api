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

[index.d.ts:17398](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17398)

___

### id

• **id**: `string`

The unique id of ActionViewItem control.

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[id](codearts_plugin_.ui.Component.md#id)

#### Defined in

[index.d.ts:17393](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17393)

___

### ideuiModule

• **ideuiModule**: `string`

The frontend module name corresponding to this control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[ideuiModule](codearts_plugin_.ui.Component.md#ideuimodule)

#### Defined in

[index.d.ts:17292](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17292)

___

### onClick

• **onClick**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Callback when a ActionViewItem is clicked.

#### Defined in

[index.d.ts:17408](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17408)

___

### onConnected

• **onConnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is mounted in front-end dom.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[onConnected](codearts_plugin_.ui.Component.md#onconnected)

#### Defined in

[index.d.ts:17302](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17302)

___

### onDisconnected

• **onDisconnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is unmounted in front-end dom.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[onDisconnected](codearts_plugin_.ui.Component.md#ondisconnected)

#### Defined in

[index.d.ts:17307](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17307)

___

### options

• **options**: [`ActionViewItemOptions`](codearts_plugin_.ui.ActionViewItemOptions.md)

Configuration parameters of the ActionViewItem component.

#### Defined in

[index.d.ts:17403](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17403)

## Methods

### blur

▸ **blur**(): `void`

Blur the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17428](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17428)

___

### dispose

▸ **dispose**(): `void`

Destroy the component.

#### Returns

`void`

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[dispose](codearts_plugin_.ui.Component.md#dispose)

#### Defined in

[index.d.ts:17453](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17453)

___

### focus

▸ **focus**(): `void`

Focus the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17418](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17418)

___

### isFocused

▸ **isFocused**(): `boolean`

Determine whether the current element is focused.

#### Returns

`boolean`

#### Defined in

[index.d.ts:17423](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17423)

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

[index.d.ts:17312](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17312)

___

### order

▸ **order**(): `number`

Obtains the order of the current component.

#### Returns

`number`

#### Defined in

[index.d.ts:17458](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17458)

___

### render

▸ **render**(): `void`

Render an html element from the action view item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17413](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17413)

___

### setFocusable

▸ **setFocusable**(): `void`

Event for modifying item focusable when dot is set.

#### Returns

`void`

#### Defined in

[index.d.ts:17433](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17433)

___

### updateClass

▸ **updateClass**(): `void`

Update the class of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17438](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17438)

___

### updateLabel

▸ **updateLabel**(): `void`

Update the label of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17443](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17443)

___

### updateTooltip

▸ **updateTooltip**(): `void`

Update the tooltip of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17448](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17448)
