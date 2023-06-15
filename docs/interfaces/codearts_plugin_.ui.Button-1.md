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

[index.d.ts:17322](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17322)

___

### id

• **id**: `string`

The unique id of control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[id](codearts_plugin_.ui.Component.md#id)

#### Defined in

[index.d.ts:17287](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17287)

___

### ideuiModule

• **ideuiModule**: `string`

The frontend module name corresponding to this control.

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[ideuiModule](codearts_plugin_.ui.Component.md#ideuimodule)

#### Defined in

[index.d.ts:17292](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17292)

___

### label

• **label**: `string`

Sets the button label.

#### Defined in

[index.d.ts:17327](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17327)

___

### onClick

• **onClick**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Callback when a button is clicked.

#### Defined in

[index.d.ts:17332](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17332)

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

• **options**: [`ButtonOptions`](codearts_plugin_.ui.ButtonOptions.md)

Parameters required for creating a Button component.

#### Defined in

[index.d.ts:17337](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17337)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose the control, and the module created by the frontend in browser will also be disposed together.

#### Returns

`void`

#### Inherited from

[Component](codearts_plugin_.ui.Component.md).[dispose](codearts_plugin_.ui.Component.md#dispose)

#### Defined in

[index.d.ts:17297](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17297)

___

### focus

▸ **focus**(): `void`

Focus the button.

#### Returns

`void`

#### Defined in

[index.d.ts:17342](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17342)

___

### hasFocus

▸ **hasFocus**(): `boolean`

Indicates whether the button is focused.

#### Returns

`boolean`

#### Defined in

[index.d.ts:17347](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17347)

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
