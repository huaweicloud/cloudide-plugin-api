[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / EventEmitter

# Class: EventEmitter<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).EventEmitter

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Constructors

- [constructor](codearts_plugin_.EventEmitter.md#constructor)

### Properties

- [event](codearts_plugin_.EventEmitter.md#event)

### Methods

- [dispose](codearts_plugin_.EventEmitter.md#dispose)
- [fire](codearts_plugin_.EventEmitter.md#fire)

## Constructors

### constructor

• **new EventEmitter**<`T`\>()

#### Type parameters

| Name |
| :------ |
| `T` |

## Properties

### event

• **event**: [`Event`](../interfaces/codearts_plugin_.Event.md)<`T`\>

#### Defined in

[index.d.ts:1620](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1620)

## Methods

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:1633](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1633)

___

### fire

▸ **fire**(`data`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `T` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:1628](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1628)
