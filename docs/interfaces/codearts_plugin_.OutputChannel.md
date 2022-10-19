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

[index.d.ts:6211](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6211)

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

[index.d.ts:6218](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6218)

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

[index.d.ts:6226](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6226)

___

### clear

▸ **clear**(): `void`

Removes all output from the channel.

#### Returns

`void`

#### Defined in

[index.d.ts:6238](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6238)

___

### dispose

▸ **dispose**(): `void`

Dispose and free associated resources.

#### Returns

`void`

#### Defined in

[index.d.ts:6265](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6265)

___

### hide

▸ **hide**(): `void`

Hide this channel from the UI.

#### Returns

`void`

#### Defined in

[index.d.ts:6260](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6260)

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

[index.d.ts:6233](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6233)

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

[index.d.ts:6245](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6245)

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

[index.d.ts:6255](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6255)
