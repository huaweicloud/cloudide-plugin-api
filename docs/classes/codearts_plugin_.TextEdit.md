[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEdit

# Class: TextEdit

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEdit

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TextEdit.md#constructor)

### Properties

- [newEol](codearts_plugin_.TextEdit.md#neweol)
- [newText](codearts_plugin_.TextEdit.md#newtext)
- [range](codearts_plugin_.TextEdit.md#range)

### Methods

- [delete](codearts_plugin_.TextEdit.md#delete)
- [insert](codearts_plugin_.TextEdit.md#insert)
- [replace](codearts_plugin_.TextEdit.md#replace)
- [setEndOfLine](codearts_plugin_.TextEdit.md#setendofline)

## Constructors

### constructor

• **new TextEdit**(`range`, `newText`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |
| `newText` | `string` |  |

#### Defined in

[index.d.ts:3435](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L3435)

## Properties

### newEol

• `Optional` **newEol**: [`EndOfLine`](../enums/codearts_plugin_.EndOfLine.md)

#### Defined in

[index.d.ts:3427](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L3427)

___

### newText

• **newText**: `string`

#### Defined in

[index.d.ts:3419](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L3419)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

#### Defined in

[index.d.ts:3414](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L3414)

## Methods

### delete

▸ `Static` **delete**(`range`): [`TextEdit`](codearts_plugin_.TextEdit.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |

#### Returns

[`TextEdit`](codearts_plugin_.TextEdit.md)

#### Defined in

[index.d.ts:3401](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L3401)

___

### insert

▸ `Static` **insert**(`position`, `newText`): [`TextEdit`](codearts_plugin_.TextEdit.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](codearts_plugin_.Position.md) |  |
| `newText` | `string` |  |

#### Returns

[`TextEdit`](codearts_plugin_.TextEdit.md)

#### Defined in

[index.d.ts:3393](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L3393)

___

### replace

▸ `Static` **replace**(`range`, `newText`): [`TextEdit`](codearts_plugin_.TextEdit.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |
| `newText` | `string` |  |

#### Returns

[`TextEdit`](codearts_plugin_.TextEdit.md)

#### Defined in

[index.d.ts:3384](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L3384)

___

### setEndOfLine

▸ `Static` **setEndOfLine**(`eol`): [`TextEdit`](codearts_plugin_.TextEdit.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `eol` | [`EndOfLine`](../enums/codearts_plugin_.EndOfLine.md) |  |

#### Returns

[`TextEdit`](codearts_plugin_.TextEdit.md)

#### Defined in

[index.d.ts:3409](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L3409)
