**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / EventEmitter

# Class: EventEmitter\<T>

An event emitter can be used to create and manage an [event](#Event) for others
to subscribe to. One emitter always owns one event.

Use this class if you want to provide event from within your extension, for instance
inside a [TextDocumentContentProvider](#TextDocumentContentProvider) or when providing
API to other extensions.

## Type parameters

Name |
------ |
`T` |

## Hierarchy

* **EventEmitter**

## Index

### Properties

* [event](_index_d_._plugin_.eventemitter.md#event)

### Methods

* [dispose](_index_d_._plugin_.eventemitter.md#dispose)
* [fire](_index_d_._plugin_.eventemitter.md#fire)

## Properties

### event

•  **event**: [Event](../interfaces/_index_d_._plugin_.event.md)\<T>

*Defined in [index.d.ts:1655](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1655)*

The event listeners can subscribe to.

## Methods

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:1668](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1668)*

Dispose this object and free resources.

**Returns:** void

___

### fire

▸ **fire**(`data`: T): void

*Defined in [index.d.ts:1663](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1663)*

Notify all subscribers of the [event](#EventEmitter.event). Failure
of one or more listener will not fail this function call.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`data` | T | The event object.  |

**Returns:** void
