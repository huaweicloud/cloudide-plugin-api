[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Pseudoterminal

# Interface: Pseudoterminal

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Pseudoterminal

Defines the interface of a terminal pty, enabling extensions to control a terminal.

## Table of contents

### Properties

- [onDidClose](cloudide_plugin_.Pseudoterminal.md#ondidclose)
- [onDidOverrideDimensions](cloudide_plugin_.Pseudoterminal.md#ondidoverridedimensions)
- [onDidWrite](cloudide_plugin_.Pseudoterminal.md#ondidwrite)

### Methods

- [close](cloudide_plugin_.Pseudoterminal.md#close)
- [handleInput](cloudide_plugin_.Pseudoterminal.md#handleinput)
- [open](cloudide_plugin_.Pseudoterminal.md#open)
- [setDimensions](cloudide_plugin_.Pseudoterminal.md#setdimensions)

## Properties

### onDidClose

• `Optional` **onDidClose**: [`Event`](cloudide_plugin_.Event.md)<`number` \| `void`\>

An event that when fired will close the pty.

#### Defined in

[index.d.ts:2860](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2860)

___

### onDidOverrideDimensions

• `Optional` **onDidOverrideDimensions**: [`Event`](cloudide_plugin_.Event.md)<`undefined` \| [`TerminalDimensions`](cloudide_plugin_.TerminalDimensions.md)\>

An event that when fired allows resizing the terminal.

#### Defined in

[index.d.ts:2855](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2855)

___

### onDidWrite

• **onDidWrite**: [`Event`](cloudide_plugin_.Event.md)<`string`\>

An event that when fired will write data to the terminal.

#### Defined in

[index.d.ts:2850](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2850)

## Methods

### close

▸ **close**(): `void`

Implement to handle when the terminal is closed.

#### Returns

`void`

#### Defined in

[index.d.ts:2872](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2872)

___

### handleInput

▸ `Optional` **handleInput**(`data`): `void`

Implement to handle inputting data in the terminal.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `string` | The inputting data. |

#### Returns

`void`

#### Defined in

[index.d.ts:2879](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2879)

___

### open

▸ **open**(`dimensions`): `void`

Implement to handle when the pty is opened.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dimensions` | `undefined` \| [`TerminalDimensions`](cloudide_plugin_.TerminalDimensions.md) | The dimensions of the terminal. |

#### Returns

`void`

#### Defined in

[index.d.ts:2867](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2867)

___

### setDimensions

▸ `Optional` **setDimensions**(`dimensions`): `void`

Implement to handle when the number of rows and columns changes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dimensions` | [`TerminalDimensions`](cloudide_plugin_.TerminalDimensions.md) | The new dimensions. |

#### Returns

`void`

#### Defined in

[index.d.ts:2886](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2886)
