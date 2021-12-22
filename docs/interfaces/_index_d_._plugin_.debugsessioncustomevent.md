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

*Defined in [index.d.ts:11606](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11606)*

Event specific information.

___

### event

• `Readonly` **event**: string

*Defined in [index.d.ts:11601](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11601)*

Type of event.

___

### session

• `Readonly` **session**: [DebugSession](_index_d_._plugin_.debugsession.md)

*Defined in [index.d.ts:11596](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11596)*

The [debug session](#DebugSession) for which the custom event was received.
