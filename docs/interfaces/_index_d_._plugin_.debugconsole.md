**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugConsole

# Interface: DebugConsole

Represents the debug console.

## Hierarchy

* **DebugConsole**

## Index

### Methods

* [append](_index_d_._plugin_.debugconsole.md#append)
* [appendLine](_index_d_._plugin_.debugconsole.md#appendline)

## Methods

### append

▸ **append**(`value`: string): void

*Defined in [index.d.ts:11846](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11846)*

Append the given value to the debug console.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string | A string, falsy values will not be printed.  |

**Returns:** void

___

### appendLine

▸ **appendLine**(`value`: string): void

*Defined in [index.d.ts:11854](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11854)*

Append the given value and a line feed character
to the debug console.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string | A string, falsy values will be printed.  |

**Returns:** void
