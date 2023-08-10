[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / OutputChannel

# Interface: OutputChannel

["@codearts/plugin"](../modules/_codearts_plugin_.md).OutputChannel

An output channel is a container for readonly textual information.

To get an instance of an `OutputChannel` use
[createOutputChannel](../modules/codearts_plugin_.window.md#createoutputchannel).

## Table of contents

### Properties

- [name](codearts_plugin_.OutputChannel.md#name)

### Methods

- [append](codearts_plugin_.OutputChannel.md#append)
- [appendLine](codearts_plugin_.OutputChannel.md#appendline)
- [clear](codearts_plugin_.OutputChannel.md#clear)
- [dispose](codearts_plugin_.OutputChannel.md#dispose)
- [hide](codearts_plugin_.OutputChannel.md#hide)
- [replace](codearts_plugin_.OutputChannel.md#replace)
- [show](codearts_plugin_.OutputChannel.md#show)

## Properties

### name

• `Readonly` **name**: `string`

The human-readable name of this output channel.

#### Defined in

[index.d.ts:6306](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6306)

## Methods

### append

▸ **append**(`value`): `void`

Append the given value to the channel.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | A string, falsy values will not be printed. |

#### Returns

`void`

#### Defined in

[index.d.ts:6313](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6313)

___

### appendLine

▸ **appendLine**(`value`): `void`

Append the given value and a line feed character
to the channel.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | A string, falsy values will be printed. |

#### Returns

`void`

#### Defined in

[index.d.ts:6321](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6321)

___

### clear

▸ **clear**(): `void`

Removes all output from the channel.

#### Returns

`void`

#### Defined in

[index.d.ts:6333](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6333)

___

### dispose

▸ **dispose**(): `void`

Dispose and free associated resources.

#### Returns

`void`

#### Defined in

[index.d.ts:6360](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6360)

___

### hide

▸ **hide**(): `void`

Hide this channel from the UI.

#### Returns

`void`

#### Defined in

[index.d.ts:6355](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6355)

___

### replace

▸ **replace**(`value`): `void`

Replaces all output from the channel with the given value.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | A string, falsy values will not be printed. |

#### Returns

`void`

#### Defined in

[index.d.ts:6328](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6328)

___

### show

▸ **show**(`preserveFocus?`): `void`

Reveal this channel in the UI.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `preserveFocus?` | `boolean` | When `true` the channel will not take focus. |

#### Returns

`void`

#### Defined in

[index.d.ts:6340](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6340)

▸ **show**(`column?`, `preserveFocus?`): `void`

Reveal this channel in the UI.

**`Deprecated`**

Use the overload with just one parameter (`show(preserveFocus?: boolean): void`).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `column?` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) | This argument is **deprecated** and will be ignored. |
| `preserveFocus?` | `boolean` | When `true` the channel will not take focus. |

#### Returns

`void`

#### Defined in

[index.d.ts:6350](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6350)
