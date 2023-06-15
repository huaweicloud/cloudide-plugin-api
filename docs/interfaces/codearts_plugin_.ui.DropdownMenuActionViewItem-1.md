[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / [ui](../modules/codearts_plugin_.ui.md) / DropdownMenuActionViewItem

# Interface: DropdownMenuActionViewItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).[ui](../modules/codearts_plugin_.ui.md).DropdownMenuActionViewItem

DropdownMenuActionViewItem Control.

## Hierarchy

- [`Component`](codearts_plugin_.ui.Component.md)

  ↳ **`DropdownMenuActionViewItem`**

## Table of contents

### Properties

- [action](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#action)
- [id](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#id)
- [ideuiModule](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#ideuimodule)
- [menuActions](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#menuactions)
- [onConnected](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#onconnected)
- [onDisconnected](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#ondisconnected)

### Methods

- [blur](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#blur)
- [dispose](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#dispose)
- [focus](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#focus)
- [isFocused](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#isfocused)
- [on](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#on)
- [render](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#render)
- [setFocusable](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#setfocusable)
- [updateClass](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#updateclass)
- [updateLabel](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#updatelabel)
- [updateTooltip](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md#updatetooltip)

## Properties

### action

• **action**: [`DropdownMenuInEditorOptions`](codearts_plugin_.ui.DropdownMenuInEditorOptions.md)

Action parameters.

#### Defined in

[index.d.ts:17568](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17568)

___

### id

• **id**: `string`

The unique id of DropdownMenuActionViewItem control.

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[id](codearts_plugin_.ui.Component.md#id)

#### Defined in

[index.d.ts:17563](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17563)

___

### ideuiModule

• **ideuiModule**: `string`

The frontend module name corresponding to this control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[ideuiModule](codearts_plugin_.ui.Component.md#ideuimodule)

#### Defined in

[index.d.ts:17292](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17292)

___

### menuActions

• **menuActions**: [`ActionViewItemAsDropdownMenuItemOptions`](codearts_plugin_.ui.ActionViewItemAsDropdownMenuItemOptions.md)[]

Menu action parameters.

#### Defined in

[index.d.ts:17573](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17573)

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

## Methods

### blur

▸ **blur**(): `void`

Blur the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17593](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17593)

___

### dispose

▸ **dispose**(): `void`

Destroy the component.

#### Returns

`void`

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[dispose](codearts_plugin_.ui.Component.md#dispose)

#### Defined in

[index.d.ts:17618](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17618)

___

### focus

▸ **focus**(): `void`

Focus the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17583](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17583)

___

### isFocused

▸ **isFocused**(): `boolean`

Determine whether the current element is focused.

#### Returns

`boolean`

#### Defined in

[index.d.ts:17588](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17588)

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

### render

▸ **render**(): `void`

Render an html element from the dropdownMenuActionViewItem element.

#### Returns

`void`

#### Defined in

[index.d.ts:17578](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17578)

___

### setFocusable

▸ **setFocusable**(): `void`

Event for modifying item focusable when dot is set.

#### Returns

`void`

#### Defined in

[index.d.ts:17598](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17598)

___

### updateClass

▸ **updateClass**(): `void`

Update the class of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17603](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17603)

___

### updateLabel

▸ **updateLabel**(): `void`

Update the label of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17608](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17608)

___

### updateTooltip

▸ **updateTooltip**(): `void`

Update the tooltip of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17613](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17613)
