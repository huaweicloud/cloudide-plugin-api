[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugConsole

# Interface: DebugConsole

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugConsole

Represents the debug console.

## Table of contents

### Methods

- [append](cloudide_plugin_.DebugConsole.md#append)
- [appendLine](cloudide_plugin_.DebugConsole.md#appendline)

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

[index.d.ts:9914](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9914)

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

[index.d.ts:9922](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9922)
