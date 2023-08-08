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

Sets the button invalid status.

#### Defined in

[index.d.ts:17447](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17447)

___

### id

• **id**: `string`

The unique id of control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[id](codearts_plugin_.ui.Component.md#id)

#### Defined in

[index.d.ts:17412](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17412)

___

### ideuiModule

• **ideuiModule**: `string`

The frontend module name corresponding to this control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[ideuiModule](codearts_plugin_.ui.Component.md#ideuimodule)

#### Defined in

[index.d.ts:17417](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17417)

___

### label

• **label**: `string`

Sets the button label.

#### Defined in

[index.d.ts:17452](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17452)

___

### onClick

• **onClick**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Callback when a button is clicked.

#### Defined in

[index.d.ts:17457](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17457)

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

• **options**: [`ButtonOptions`](codearts_plugin_.ui.ButtonOptions.md)

Parameters required for creating a Button component.

#### Defined in

[index.d.ts:17462](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17462)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose the control, and the module created by the frontend in browser will also be disposed together.

#### Returns

`void`

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[dispose](codearts_plugin_.ui.Component.md#dispose)

#### Defined in

[index.d.ts:17422](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17422)

___

### focus

▸ **focus**(): `void`

Focus the button.

#### Returns

`void`

#### Defined in

[index.d.ts:17467](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17467)

___

### hasFocus

▸ **hasFocus**(): `boolean`

Indicates whether the button is focused.

#### Returns

`boolean`

#### Defined in

[index.d.ts:17472](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17472)

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
