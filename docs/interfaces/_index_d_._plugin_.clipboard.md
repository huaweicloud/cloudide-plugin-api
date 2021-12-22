**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Clipboard

# Interface: Clipboard

The clipboard provides read and write access to the system's clipboard.

## Hierarchy

* **Clipboard**

## Index

### Methods

* [readText](_index_d_._plugin_.clipboard.md#readtext)
* [writeText](_index_d_._plugin_.clipboard.md#writetext)

## Methods

### readText

▸ **readText**(): [Thenable](_index_d_.thenable.md)\<string>

*Defined in [index.d.ts:7957](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7957)*

Read the current clipboard contents as text.

**Returns:** [Thenable](_index_d_.thenable.md)\<string>

A thenable that resolves to a string.

___

### writeText

▸ **writeText**(`value`: string): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7963](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7963)*

Writes text into the clipboard.

#### Parameters:

Name | Type |
------ | ------ |
`value` | string |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

A thenable that resolves when writing happened.
