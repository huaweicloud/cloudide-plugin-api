[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Clipboard

# Interface: Clipboard

["@codearts/plugin"](../modules/_codearts_plugin_.md).Clipboard

The clipboard provides read and write access to the system's clipboard.

## Table of contents

### Methods

- [readText](codearts_plugin_.Clipboard.md#readtext)
- [writeText](codearts_plugin_.Clipboard.md#writetext)

## Methods

### readText

▸ **readText**(): [`Thenable`](Thenable.md)<`string`\>

Read the current clipboard contents as text.

#### Returns

[`Thenable`](Thenable.md)<`string`\>

A thenable that resolves to a string.

#### Defined in

[index.d.ts:9079](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L9079)

___

### writeText

▸ **writeText**(`value`): [`Thenable`](Thenable.md)<`void`\>

Writes text into the clipboard.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

A thenable that resolves when writing happened.

#### Defined in

[index.d.ts:9085](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L9085)
