[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Selection

# Class: Selection

["@codearts/plugin"](../modules/_codearts_plugin_.md).Selection

## Hierarchy

- [`Range`](codearts_plugin_.Range.md)

  ↳ **`Selection`**

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Selection.md#constructor)

### Properties

- [active](codearts_plugin_.Selection.md#active)
- [anchor](codearts_plugin_.Selection.md#anchor)
- [end](codearts_plugin_.Selection.md#end)
- [isEmpty](codearts_plugin_.Selection.md#isempty)
- [isReversed](codearts_plugin_.Selection.md#isreversed)
- [isSingleLine](codearts_plugin_.Selection.md#issingleline)
- [start](codearts_plugin_.Selection.md#start)

### Methods

- [contains](codearts_plugin_.Selection.md#contains)
- [intersection](codearts_plugin_.Selection.md#intersection)
- [isEqual](codearts_plugin_.Selection.md#isequal)
- [union](codearts_plugin_.Selection.md#union)
- [with](codearts_plugin_.Selection.md#with)

## Constructors

### constructor

• **new Selection**(`anchor`, `active`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `anchor` | [`Position`](codearts_plugin_.Position.md) |  |
| `active` | [`Position`](codearts_plugin_.Position.md) |  |

#### Overrides

[Range](codearts_plugin_.Range.md).[constructor](codearts_plugin_.Range.md#constructor)

#### Defined in

[index.d.ts:499](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L499)

• **new Selection**(`anchorLine`, `anchorCharacter`, `activeLine`, `activeCharacter`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `anchorLine` | `number` |  |
| `anchorCharacter` | `number` |  |
| `activeLine` | `number` |  |
| `activeCharacter` | `number` |  |

#### Overrides

[Range](codearts_plugin_.Range.md).[constructor](codearts_plugin_.Range.md#constructor)

#### Defined in

[index.d.ts:509](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L509)

## Properties

### active

• **active**: [`Position`](codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:491](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L491)

___

### anchor

• **anchor**: [`Position`](codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:485](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L485)

___

### end

• `Readonly` **end**: [`Position`](codearts_plugin_.Position.md)

#### Inherited from

[Range](codearts_plugin_.Range.md).[end](codearts_plugin_.Range.md#end)

#### Defined in

[index.d.ts:388](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L388)

___

### isEmpty

• **isEmpty**: `boolean`

#### Inherited from

[Range](codearts_plugin_.Range.md).[isEmpty](codearts_plugin_.Range.md#isempty)

#### Defined in

[index.d.ts:413](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L413)

___

### isReversed

• **isReversed**: `boolean`

#### Defined in

[index.d.ts:514](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L514)

___

### isSingleLine

• **isSingleLine**: `boolean`

#### Inherited from

[Range](codearts_plugin_.Range.md).[isSingleLine](codearts_plugin_.Range.md#issingleline)

#### Defined in

[index.d.ts:418](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L418)

___

### start

• `Readonly` **start**: [`Position`](codearts_plugin_.Position.md)

#### Inherited from

[Range](codearts_plugin_.Range.md).[start](codearts_plugin_.Range.md#start)

#### Defined in

[index.d.ts:383](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L383)

## Methods

### contains

▸ **contains**(`positionOrRange`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `positionOrRange` | [`Range`](codearts_plugin_.Range.md) \| [`Position`](codearts_plugin_.Position.md) |  |

#### Returns

`boolean`

#### Inherited from

[Range](codearts_plugin_.Range.md).[contains](codearts_plugin_.Range.md#contains)

#### Defined in

[index.d.ts:427](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L427)

___

### intersection

▸ **intersection**(`range`): `undefined` \| [`Range`](codearts_plugin_.Range.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |

#### Returns

`undefined` \| [`Range`](codearts_plugin_.Range.md)

#### Inherited from

[Range](codearts_plugin_.Range.md).[intersection](codearts_plugin_.Range.md#intersection)

#### Defined in

[index.d.ts:446](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L446)

___

### isEqual

▸ **isEqual**(`other`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Range`](codearts_plugin_.Range.md) |  |

#### Returns

`boolean`

#### Inherited from

[Range](codearts_plugin_.Range.md).[isEqual](codearts_plugin_.Range.md#isequal)

#### Defined in

[index.d.ts:436](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L436)

___

### union

▸ **union**(`other`): [`Range`](codearts_plugin_.Range.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Range`](codearts_plugin_.Range.md) |  |

#### Returns

[`Range`](codearts_plugin_.Range.md)

#### Inherited from

[Range](codearts_plugin_.Range.md).[union](codearts_plugin_.Range.md#union)

#### Defined in

[index.d.ts:454](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L454)

___

### with

▸ **with**(`start?`, `end?`): [`Range`](codearts_plugin_.Range.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start?` | [`Position`](codearts_plugin_.Position.md) |  |
| `end?` | [`Position`](codearts_plugin_.Position.md) |  |

#### Returns

[`Range`](codearts_plugin_.Range.md)

#### Inherited from

[Range](codearts_plugin_.Range.md).[with](codearts_plugin_.Range.md#with)

#### Defined in

[index.d.ts:464](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L464)

▸ **with**(`change`): [`Range`](codearts_plugin_.Range.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` |  |
| `change.end?` | [`Position`](codearts_plugin_.Position.md) | - |
| `change.start?` | [`Position`](codearts_plugin_.Position.md) | - |

#### Returns

[`Range`](codearts_plugin_.Range.md)

#### Inherited from

[Range](codearts_plugin_.Range.md).[with](codearts_plugin_.Range.md#with)

#### Defined in

[index.d.ts:473](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L473)
