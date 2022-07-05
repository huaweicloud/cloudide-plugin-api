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

[index.d.ts:10659](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10659)

___

### onDidClose

• `Optional` **onDidClose**: [`Event`](codearts_plugin_.Event.md)<`number` \| `void`\>

#### Defined in

[index.d.ts:10639](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10639)

___

### onDidOverrideDimensions

• `Optional` **onDidOverrideDimensions**: [`Event`](codearts_plugin_.Event.md)<`undefined` \| [`TerminalDimensions`](codearts_plugin_.TerminalDimensions.md)\>

#### Defined in

[index.d.ts:10608](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10608)

___

### onDidWrite

• **onDidWrite**: [`Event`](codearts_plugin_.Event.md)<`string`\>

#### Defined in

[index.d.ts:10580](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10580)

## Methods

### close

▸ **close**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:10672](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10672)

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

[index.d.ts:10694](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10694)

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

[index.d.ts:10667](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10667)

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

[index.d.ts:10709](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10709)
