[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / OutputChannel

# Interface: OutputChannel

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).OutputChannel

An output channel is a container for readonly textual information.

## Table of contents

### Properties

- [name](cloudide_plugin_.OutputChannel.md#name)

### Methods

- [append](cloudide_plugin_.OutputChannel.md#append)
- [appendLine](cloudide_plugin_.OutputChannel.md#appendline)
- [clear](cloudide_plugin_.OutputChannel.md#clear)
- [dispose](cloudide_plugin_.OutputChannel.md#dispose)
- [hide](cloudide_plugin_.OutputChannel.md#hide)
- [show](cloudide_plugin_.OutputChannel.md#show)

## Properties

### name

• `Readonly` **name**: `string`

The name of this output channel.

#### Defined in

[index.d.ts:2600](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2600)

## Methods

### append

▸ **append**(`value`): `void`

Append the given value to the channel.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Defined in

[index.d.ts:2607](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2607)

___

### appendLine

▸ **appendLine**(`value`): `void`

Append the given value and a line feed character
to the channel.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Defined in

[index.d.ts:2615](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2615)

___

### clear

▸ **clear**(): `void`

Removes all output from the channel.

#### Returns

`void`

#### Defined in

[index.d.ts:2620](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2620)

___

### dispose

▸ **dispose**(): `void`

Dispose and free associated resources.

#### Returns

`void`

#### Defined in

[index.d.ts:2637](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2637)

___

### hide

▸ **hide**(): `void`

Hide this channel from the UI.

#### Returns

`void`

#### Defined in

[index.d.ts:2632](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2632)

___

### show

▸ **show**(`preserveFocus?`): `void`

Reveal this channel in the UI.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `preserveFocus?` | `boolean` | When 'true' the channel will not take focus. |

#### Returns

`void`

#### Defined in

[index.d.ts:2627](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2627)
