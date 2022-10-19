[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / [ui](../modules/codearts_plugin_.ui.md) / Button

# Interface: Button

["@codearts/plugin"](../modules/_codearts_plugin_.md).[ui](../modules/codearts_plugin_.ui.md).Button

Button Control.

## Hierarchy

- [`Component`](codearts_plugin_.ui.Component.md)

  ↳ **`Button`**

## Table of contents

### Properties

- [enabled](codearts_plugin_.ui.Button-1.md#enabled)
- [id](codearts_plugin_.ui.Button-1.md#id)
- [ideuiModule](codearts_plugin_.ui.Button-1.md#ideuimodule)
- [label](codearts_plugin_.ui.Button-1.md#label)
- [onClick](codearts_plugin_.ui.Button-1.md#onclick)
- [onConnected](codearts_plugin_.ui.Button-1.md#onconnected)
- [onDisconnected](codearts_plugin_.ui.Button-1.md#ondisconnected)
- [options](codearts_plugin_.ui.Button-1.md#options)

### Methods

- [dispose](codearts_plugin_.ui.Button-1.md#dispose)
- [focus](codearts_plugin_.ui.Button-1.md#focus)
- [hasFocus](codearts_plugin_.ui.Button-1.md#hasfocus)
- [on](codearts_plugin_.ui.Button-1.md#on)

## Properties

### enabled

• **enabled**: `boolean`

#### Defined in

[index.d.ts:16441](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16441)

___

### id

• **id**: `string`

The unique id of control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[id](codearts_plugin_.ui.Component.md#id)

#### Defined in

[index.d.ts:16409](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16409)

___

### ideuiModule

• **ideuiModule**: `string`

The frontend module name corresponding to this control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[ideuiModule](codearts_plugin_.ui.Component.md#ideuimodule)

#### Defined in

[index.d.ts:16414](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16414)

___

### label

• **label**: `string`

#### Defined in

[index.d.ts:16442](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16442)

___

### onClick

• **onClick**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:16443](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16443)

___

### onConnected

• **onConnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is mounted in front-end dom.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[onConnected](codearts_plugin_.ui.Component.md#onconnected)

#### Defined in

[index.d.ts:16424](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16424)

___

### onDisconnected

• **onDisconnected**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the control is unmounted in front-end dom.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[onDisconnected](codearts_plugin_.ui.Component.md#ondisconnected)

#### Defined in

[index.d.ts:16429](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16429)

___

### options

• **options**: [`ButtonOptions`](codearts_plugin_.ui.ButtonOptions.md)

#### Defined in

[index.d.ts:16444](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16444)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose the control, and the module created by the frontend in browser will also be disposed together.

#### Returns

`void`

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[dispose](codearts_plugin_.ui.Component.md#dispose)

#### Defined in

[index.d.ts:16419](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16419)

___

### focus

▸ **focus**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:16445](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16445)

___

### hasFocus

▸ **hasFocus**(): `boolean`

#### Returns

`boolean`

#### Defined in

[index.d.ts:16446](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16446)

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

[index.d.ts:16434](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16434)
