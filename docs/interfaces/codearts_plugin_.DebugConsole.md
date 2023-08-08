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

[index.d.ts:15334](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15334)

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

[index.d.ts:15342](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15342)
