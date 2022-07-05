[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextDocument

# Interface: TextDocument

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextDocument

## Table of contents

### Properties

- [eol](codearts_plugin_.TextDocument.md#eol)
- [fileName](codearts_plugin_.TextDocument.md#filename)
- [isClosed](codearts_plugin_.TextDocument.md#isclosed)
- [isDirty](codearts_plugin_.TextDocument.md#isdirty)
- [isUntitled](codearts_plugin_.TextDocument.md#isuntitled)
- [languageId](codearts_plugin_.TextDocument.md#languageid)
- [lineCount](codearts_plugin_.TextDocument.md#linecount)
- [uri](codearts_plugin_.TextDocument.md#uri)
- [version](codearts_plugin_.TextDocument.md#version)

### Methods

- [getText](codearts_plugin_.TextDocument.md#gettext)
- [getWordRangeAtPosition](codearts_plugin_.TextDocument.md#getwordrangeatposition)
- [lineAt](codearts_plugin_.TextDocument.md#lineat)
- [offsetAt](codearts_plugin_.TextDocument.md#offsetat)
- [positionAt](codearts_plugin_.TextDocument.md#positionat)
- [save](codearts_plugin_.TextDocument.md#save)
- [validatePosition](codearts_plugin_.TextDocument.md#validateposition)
- [validateRange](codearts_plugin_.TextDocument.md#validaterange)

## Properties

### eol

• `Readonly` **eol**: [`EndOfLine`](../enums/codearts_plugin_.EndOfLine.md)

#### Defined in

[index.d.ts:156](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L156)

___

### fileName

• `Readonly` **fileName**: `string`

#### Defined in

[index.d.ts:113](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L113)

___

### isClosed

• `Readonly` **isClosed**: `boolean`

#### Defined in

[index.d.ts:142](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L142)

___

### isDirty

• `Readonly` **isDirty**: `boolean`

#### Defined in

[index.d.ts:136](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L136)

___

### isUntitled

• `Readonly` **isUntitled**: `boolean`

#### Defined in

[index.d.ts:120](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L120)

___

### languageId

• `Readonly` **languageId**: `string`

#### Defined in

[index.d.ts:125](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L125)

___

### lineCount

• `Readonly` **lineCount**: `number`

#### Defined in

[index.d.ts:161](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L161)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:107](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L107)

___

### version

• `Readonly` **version**: `number`

#### Defined in

[index.d.ts:131](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L131)

## Methods

### getText

▸ **getText**(`range?`): `string`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range?` | [`Range`](../classes/codearts_plugin_.Range.md) |  |

#### Returns

`string`

#### Defined in

[index.d.ts:212](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L212)

___

### getWordRangeAtPosition

▸ **getWordRangeAtPosition**(`position`, `regex?`): `undefined` \| [`Range`](../classes/codearts_plugin_.Range.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `regex?` | `RegExp` |  |

#### Returns

`undefined` \| [`Range`](../classes/codearts_plugin_.Range.md)

#### Defined in

[index.d.ts:232](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L232)

___

### lineAt

▸ **lineAt**(`line`): [`TextLine`](codearts_plugin_.TextLine.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `line` | `number` |  |

#### Returns

[`TextLine`](codearts_plugin_.TextLine.md)

#### Defined in

[index.d.ts:171](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L171)

▸ **lineAt**(`position`): [`TextLine`](codearts_plugin_.TextLine.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |

#### Returns

[`TextLine`](codearts_plugin_.TextLine.md)

#### Defined in

[index.d.ts:185](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L185)

___

### offsetAt

▸ **offsetAt**(`position`): `number`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |

#### Returns

`number`

#### Defined in

[index.d.ts:195](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L195)

___

### positionAt

▸ **positionAt**(`offset`): [`Position`](../classes/codearts_plugin_.Position.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `offset` | `number` |  |

#### Returns

[`Position`](../classes/codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:203](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L203)

___

### save

▸ **save**(): [`Thenable`](Thenable.md)<`boolean`\>

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:150](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L150)

___

### validatePosition

▸ **validatePosition**(`position`): [`Position`](../classes/codearts_plugin_.Position.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |

#### Returns

[`Position`](../classes/codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:248](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L248)

___

### validateRange

▸ **validateRange**(`range`): [`Range`](../classes/codearts_plugin_.Range.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) |  |

#### Returns

[`Range`](../classes/codearts_plugin_.Range.md)

#### Defined in

[index.d.ts:240](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L240)
