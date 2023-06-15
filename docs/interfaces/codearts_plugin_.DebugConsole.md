[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugConsole

# Interface: DebugConsole

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugConsole

Represents the debug console.

## Table of contents

### Methods

- [append](codearts_plugin_.DebugConsole.md#append)
- [appendLine](codearts_plugin_.DebugConsole.md#appendline)

## Methods

### append

▸ **append**(`value`): `void`

Append the given value to the debug console.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | A string, falsy values will not be printed. |

#### Returns

`void`

#### Defined in

[index.d.ts:15231](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L15231)

___

### appendLine

▸ **appendLine**(`value`): `void`

Append the given value and a line feed character
to the debug console.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | A string, falsy values will be printed. |

#### Returns

`void`

#### Defined in

[index.d.ts:15239](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L15239)
