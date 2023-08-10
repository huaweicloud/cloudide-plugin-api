[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / EventEmitter

# Class: EventEmitter<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).EventEmitter

An event emitter can be used to create and manage an [Event](../interfaces/codearts_plugin_.Event.md) for others
to subscribe to. One emitter always owns one event.

Use this class if you want to provide event from within your extension, for instance
inside a [TextDocumentContentProvider](../interfaces/codearts_plugin_.TextDocumentContentProvider.md) or when providing
API to other extensions.

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

The event listeners can subscribe to.

#### Defined in

[index.d.ts:1620](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1620)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this object and free resources.

#### Returns

`void`

#### Defined in

[index.d.ts:1633](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1633)

___

### fire

▸ **fire**(`data`): `void`

Notify all subscribers of the [event](codearts_plugin_.EventEmitter.md#event). Failure
of one or more listener will not fail this function call.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `T` | The event object. |

#### Returns

`void`

#### Defined in

[index.d.ts:1628](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1628)
