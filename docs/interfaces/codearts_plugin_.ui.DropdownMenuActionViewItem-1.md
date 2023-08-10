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

[index.d.ts:17677](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17677)

___

### id

• **id**: `string`

The unique id of DropdownMenuActionViewItem control.

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[id](codearts_plugin_.ui.Component.md#id)

#### Defined in

[index.d.ts:17672](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17672)

___

### ideuiModule

• **ideuiModule**: `string`

The frontend module name corresponding to this control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[ideuiModule](codearts_plugin_.ui.Component.md#ideuimodule)

#### Defined in

[index.d.ts:17401](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17401)

___

### menuActions

• **menuActions**: [`ActionViewItemAsDropdownMenuItemOptions`](codearts_plugin_.ui.ActionViewItemAsDropdownMenuItemOptions.md)[]

Menu action parameters.

#### Defined in

[index.d.ts:17682](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17682)

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

## Methods

### blur

▸ **blur**(): `void`

Blur the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17702](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17702)

___

### dispose

▸ **dispose**(): `void`

Destroy the component.

#### Returns

`void`

#### Overrides

[Component](codearts_plugin_.ui.Component.md).[dispose](codearts_plugin_.ui.Component.md#dispose)

#### Defined in

[index.d.ts:17727](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17727)

___

### focus

▸ **focus**(): `void`

Focus the current item element.

#### Returns

`void`

#### Defined in

[index.d.ts:17692](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17692)

___

### isFocused

▸ **isFocused**(): `boolean`

Determine whether the current element is focused.

#### Returns

`boolean`

#### Defined in

[index.d.ts:17697](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17697)

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

### render

▸ **render**(): `void`

Render an html element from the dropdownMenuActionViewItem element.

#### Returns

`void`

#### Defined in

[index.d.ts:17687](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17687)

___

### setFocusable

▸ **setFocusable**(): `void`

Event for modifying item focusable when dot is set.

#### Returns

`void`

#### Defined in

[index.d.ts:17707](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17707)

___

### updateClass

▸ **updateClass**(): `void`

Update the class of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17712](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17712)

___

### updateLabel

▸ **updateLabel**(): `void`

Update the label of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17717](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17717)

___

### updateTooltip

▸ **updateTooltip**(): `void`

Update the tooltip of the current item.

#### Returns

`void`

#### Defined in

[index.d.ts:17722](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17722)
