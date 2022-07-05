[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Range

# Class: Range

["@codearts/plugin"](../modules/_codearts_plugin_.md).Range

## Hierarchy

- **`Range`**

  ↳ [`Selection`](codearts_plugin_.Selection.md)

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Range.md#constructor)

### Properties

- [end](codearts_plugin_.Range.md#end)
- [isEmpty](codearts_plugin_.Range.md#isempty)
- [isSingleLine](codearts_plugin_.Range.md#issingleline)
- [start](codearts_plugin_.Range.md#start)

### Methods

- [contains](codearts_plugin_.Range.md#contains)
- [intersection](codearts_plugin_.Range.md#intersection)
- [isEqual](codearts_plugin_.Range.md#isequal)
- [union](codearts_plugin_.Range.md#union)
- [with](codearts_plugin_.Range.md#with)

## Constructors

### constructor

• **new Range**(`start`, `end`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | [`Position`](codearts_plugin_.Position.md) |  |
| `end` | [`Position`](codearts_plugin_.Position.md) |  |

#### Defined in

[index.d.ts:397](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L397)

• **new Range**(`startLine`, `startCharacter`, `endLine`, `endCharacter`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startLine` | `number` |  |
| `startCharacter` | `number` |  |
| `endLine` | `number` |  |
| `endCharacter` | `number` |  |

#### Defined in

[index.d.ts:408](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L408)

## Properties

### end

• `Readonly` **end**: [`Position`](codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:388](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L388)

___

### isEmpty

• **isEmpty**: `boolean`

#### Defined in

[index.d.ts:413](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L413)

___

### isSingleLine

• **isSingleLine**: `boolean`

#### Defined in

[index.d.ts:418](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L418)

___

### start

• `Readonly` **start**: [`Position`](codearts_plugin_.Position.md)

#### Defined in

[index.d.ts:383](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L383)

## Methods

### contains

▸ **contains**(`positionOrRange`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `positionOrRange` | [`Range`](codearts_plugin_.Range.md) \| [`Position`](codearts_plugin_.Position.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:427](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L427)

___

### intersection

▸ **intersection**(`range`): `undefined` \| [`Range`](codearts_plugin_.Range.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |

#### Returns

`undefined` \| [`Range`](codearts_plugin_.Range.md)

#### Defined in

[index.d.ts:446](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L446)

___

### isEqual

▸ **isEqual**(`other`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Range`](codearts_plugin_.Range.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:436](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L436)

___

### union

▸ **union**(`other`): [`Range`](codearts_plugin_.Range.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Range`](codearts_plugin_.Range.md) |  |

#### Returns

[`Range`](codearts_plugin_.Range.md)

#### Defined in

[index.d.ts:454](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L454)

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

#### Defined in

[index.d.ts:464](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L464)

▸ **with**(`change`): [`Range`](codearts_plugin_.Range.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` |  |
| `change.end?` | [`Position`](codearts_plugin_.Position.md) | - |
| `change.start?` | [`Position`](codearts_plugin_.Position.md) | - |

#### Returns

[`Range`](codearts_plugin_.Range.md)

#### Defined in

[index.d.ts:473](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L473)
