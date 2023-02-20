**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugSessionCustomEvent

# Interface: DebugSessionCustomEvent

A custom Debug Adapter Protocol event received from a [debug session](#DebugSession).

## Hierarchy

* **DebugSessionCustomEvent**

## Index

### Properties

* [body](_index_d_._plugin_.debugsessioncustomevent.md#body)
* [event](_index_d_._plugin_.debugsessioncustomevent.md#event)
* [session](_index_d_._plugin_.debugsessioncustomevent.md#session)

## Properties

### body

• `Optional` `Readonly` **body**: any

*Defined in [index.d.ts:11626](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11626)*

Event specific information.

___

### event

• `Readonly` **event**: string

*Defined in [index.d.ts:11621](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11621)*

Type of event.

___

### session

• `Readonly` **session**: [DebugSession](_index_d_._plugin_.debugsession.md)

*Defined in [index.d.ts:11616](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11616)*

The [debug session](#DebugSession) for which the custom event was received.
