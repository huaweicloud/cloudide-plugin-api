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

[index.d.ts:14793](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L14793)

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

[index.d.ts:14801](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L14801)
