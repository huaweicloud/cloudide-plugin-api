[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / [ui](../modules/codearts_plugin_.ui.md) / Component

# Interface: Component

["@codearts/plugin"](../modules/_codearts_plugin_.md).[ui](../modules/codearts_plugin_.ui.md).Component

## Hierarchy

- **`Component`**

  ↳ [`Button`](codearts_plugin_.ui.Button-1.md)

  ↳ [`ActionViewItem`](codearts_plugin_.ui.ActionViewItem-1.md)

  ↳ [`DropdownMenuActionViewItem`](codearts_plugin_.ui.DropdownMenuActionViewItem-1.md)

## Table of contents

### Properties

- [id](codearts_plugin_.ui.Component.md#id)
- [ideuiModule](codearts_plugin_.ui.Component.md#ideuimodule)
- [onConnected](codearts_plugin_.ui.Component.md#onconnected)
- [onDisconnected](codearts_plugin_.ui.Component.md#ondisconnected)

### Methods

- [dispose](codearts_plugin_.ui.Component.md#dispose)
- [on](codearts_plugin_.ui.Component.md#on)

## Properties

### id

• **id**: `string`

The unique id of control.

#### Defined in

[index.d.ts:17199](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17199)

___

### ideuiModule

• **ideuiModule**: `string`

The frontend module name corresponding to this control.

#### Defined in

[index.d.ts:17204](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17204)

___

### onConnected

• **onConnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is mounted in front-end dom.

#### Defined in

[index.d.ts:17214](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17214)

___

### onDisconnected

• **onDisconnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is unmounted in front-end dom.

#### Defined in

[index.d.ts:17219](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17219)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose the control, and the module created by the frontend in browser will also be disposed together.

#### Returns

`void`

#### Defined in

[index.d.ts:17209](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17209)

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

#### Defined in

[index.d.ts:17224](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17224)
