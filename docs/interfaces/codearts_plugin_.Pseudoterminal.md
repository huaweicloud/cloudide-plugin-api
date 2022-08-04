[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Pseudoterminal

# Interface: Pseudoterminal

["@codearts/plugin"](../modules/_codearts_plugin_.md).Pseudoterminal

## Table of contents

### Properties

- [onDidChangeName](codearts_plugin_.Pseudoterminal.md#ondidchangename)
- [onDidClose](codearts_plugin_.Pseudoterminal.md#ondidclose)
- [onDidOverrideDimensions](codearts_plugin_.Pseudoterminal.md#ondidoverridedimensions)
- [onDidWrite](codearts_plugin_.Pseudoterminal.md#ondidwrite)

### Methods

- [close](codearts_plugin_.Pseudoterminal.md#close)
- [handleInput](codearts_plugin_.Pseudoterminal.md#handleinput)
- [open](codearts_plugin_.Pseudoterminal.md#open)
- [setDimensions](codearts_plugin_.Pseudoterminal.md#setdimensions)

## Properties

### onDidChangeName

• `Optional` **onDidChangeName**: [`Event`](codearts_plugin_.Event.md)<`string`\>

#### Defined in

[index.d.ts:10689](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10689)

___

### onDidClose

• `Optional` **onDidClose**: [`Event`](codearts_plugin_.Event.md)<`number` \| `void`\>

#### Defined in

[index.d.ts:10669](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10669)

___

### onDidOverrideDimensions

• `Optional` **onDidOverrideDimensions**: [`Event`](codearts_plugin_.Event.md)<`undefined` \| [`TerminalDimensions`](codearts_plugin_.TerminalDimensions.md)\>

#### Defined in

[index.d.ts:10638](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10638)

___

### onDidWrite

• **onDidWrite**: [`Event`](codearts_plugin_.Event.md)<`string`\>

#### Defined in

[index.d.ts:10610](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10610)

## Methods

### close

▸ **close**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:10702](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10702)

___

### handleInput

▸ `Optional` **handleInput**(`data`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `string` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:10724](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10724)

___

### open

▸ **open**(`initialDimensions`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `initialDimensions` | `undefined` \| [`TerminalDimensions`](codearts_plugin_.TerminalDimensions.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:10697](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10697)

___

### setDimensions

▸ `Optional` **setDimensions**(`dimensions`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dimensions` | [`TerminalDimensions`](codearts_plugin_.TerminalDimensions.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:10739](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10739)
