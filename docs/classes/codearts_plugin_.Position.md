[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Position

# Class: Position

["@codearts/plugin"](../modules/_codearts_plugin_.md).Position

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Position.md#constructor)

### Properties

- [character](codearts_plugin_.Position.md#character)
- [line](codearts_plugin_.Position.md#line)

### Methods

- [compareTo](codearts_plugin_.Position.md#compareto)
- [isAfter](codearts_plugin_.Position.md#isafter)
- [isAfterOrEqual](codearts_plugin_.Position.md#isafterorequal)
- [isBefore](codearts_plugin_.Position.md#isbefore)
- [isBeforeOrEqual](codearts_plugin_.Position.md#isbeforeorequal)
- [isEqual](codearts_plugin_.Position.md#isequal)
- [translate](codearts_plugin_.Position.md#translate)
- [with](codearts_plugin_.Position.md#with)

## Constructors

### constructor

• **new Position**(`line`, `character`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `line` | `number` |  |
| `character` | `number` |  |

#### Defined in

[index.d.ts:275](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L275)

## Properties

### character

• `Readonly` **character**: `number`

#### Defined in

[index.d.ts:269](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L269)

___

### line

• `Readonly` **line**: `number`

#### Defined in

[index.d.ts:264](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L264)

## Methods

### compareTo

▸ **compareTo**(`other`): `number`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) |  |

#### Returns

`number`

#### Defined in

[index.d.ts:330](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L330)

___

### isAfter

▸ **isAfter**(`other`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:302](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L302)

___

### isAfterOrEqual

▸ **isAfterOrEqual**(`other`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:311](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L311)

___

### isBefore

▸ **isBefore**(`other`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:284](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L284)

___

### isBeforeOrEqual

▸ **isBeforeOrEqual**(`other`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:293](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L293)

___

### isEqual

▸ **isEqual**(`other`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:320](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L320)

___

### translate

▸ **translate**(`lineDelta?`, `characterDelta?`): [`Position`](codearts_plugin_.Position.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `lineDelta?` | `number` |  |
| `characterDelta?` | `number` |  |

#### Returns

[`Position`](codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:340](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L340)

▸ **translate**(`change`): [`Position`](codearts_plugin_.Position.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` |  |
| `change.characterDelta?` | `number` | - |
| `change.lineDelta?` | `number` | - |

#### Returns

[`Position`](codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:349](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L349)

___

### with

▸ **with**(`line?`, `character?`): [`Position`](codearts_plugin_.Position.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `line?` | `number` |  |
| `character?` | `number` |  |

#### Returns

[`Position`](codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:358](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L358)

▸ **with**(`change`): [`Position`](codearts_plugin_.Position.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` |  |
| `change.character?` | `number` | - |
| `change.line?` | `number` | - |

#### Returns

[`Position`](codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:367](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L367)
