[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / EventEmitter

# Class: EventEmitter<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).EventEmitter

An event emitter used to create and fire an [event](#Event) or to subscribe to.

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.EventEmitter.md#constructor)

### Properties

- [event](cloudide_plugin_.EventEmitter.md#event)

### Methods

- [dispose](cloudide_plugin_.EventEmitter.md#dispose)
- [fire](cloudide_plugin_.EventEmitter.md#fire)

## Constructors

### constructor

• **new EventEmitter**<`T`\>()

#### Type parameters

| Name |
| :------ |
| `T` |

## Properties

### event

• **event**: [`Event`](../interfaces/cloudide_plugin_.Event.md)<`T`\>

The event listeners can subscribe to

#### Defined in

[index.d.ts:2036](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2036)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this object

#### Returns

`void`

#### Defined in

[index.d.ts:2047](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2047)

___

### fire

▸ **fire**(`data?`): `void`

Fire the event and pass data object

#### Parameters

| Name | Type |
| :------ | :------ |
| `data?` | `T` |

#### Returns

`void`

#### Defined in

[index.d.ts:2042](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2042)
