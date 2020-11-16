**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugAdapter

# Interface: DebugAdapter

A debug adapter that implements the Debug Adapter Protocol can be registered with VS Code if it implements the DebugAdapter interface.

## Hierarchy

* [Disposable](../classes/_index_d_._plugin_.disposable.md)

  ↳ **DebugAdapter**

## Index

### Constructors

* [constructor](_index_d_._plugin_.debugadapter.md#constructor)

### Properties

* [onDidSendMessage](_index_d_._plugin_.debugadapter.md#ondidsendmessage)

### Methods

* [dispose](_index_d_._plugin_.debugadapter.md#dispose)
* [handleMessage](_index_d_._plugin_.debugadapter.md#handlemessage)
* [from](_index_d_._plugin_.debugadapter.md#from)

## Constructors

### constructor

\+ **new DebugAdapter**(`callOnDispose`: Function): [DebugAdapter](_index_d_._plugin_.debugadapter.md)

*Inherited from [Disposable](../classes/_index_d_._plugin_.disposable.md).[constructor](../classes/_index_d_._plugin_.disposable.md#constructor)*

*Defined in [index.d.ts:1465](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1465)*

Creates a new Disposable calling the provided function
on dispose.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`callOnDispose` | Function | Function that disposes something.  |

**Returns:** [DebugAdapter](_index_d_._plugin_.debugadapter.md)

## Properties

### onDidSendMessage

• `Readonly` **onDidSendMessage**: [Event](_index_d_._plugin_.event.md)\<[DebugProtocolMessage](_index_d_._plugin_.debugprotocolmessage.md)>

*Defined in [index.d.ts:10296](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10296)*

An event which fires after the debug adapter has sent a Debug Adapter Protocol message to VS Code.
Messages can be requests, responses, or events.

## Methods

### dispose

▸ **dispose**(): any

*Inherited from [Disposable](../classes/_index_d_._plugin_.disposable.md).[dispose](../classes/_index_d_._plugin_.disposable.md#dispose)*

*Defined in [index.d.ts:1477](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1477)*

Dispose this object.

**Returns:** any

___

### handleMessage

▸ **handleMessage**(`message`: [DebugProtocolMessage](_index_d_._plugin_.debugprotocolmessage.md)): void

*Defined in [index.d.ts:10304](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10304)*

Handle a Debug Adapter Protocol message.
Messages can be requests, responses, or events.
Results or errors are returned via onSendMessage events.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | [DebugProtocolMessage](_index_d_._plugin_.debugprotocolmessage.md) | A Debug Adapter Protocol message  |

**Returns:** void

___

### from

▸ `Static`**from**(...`disposableLikes`: { dispose: () => any  }[]): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Inherited from [Disposable](../classes/_index_d_._plugin_.disposable.md).[from](../classes/_index_d_._plugin_.disposable.md#from)*

*Defined in [index.d.ts:1465](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1465)*

Combine many disposable-likes into one. Use this method
when having objects with a dispose function which are not
instances of Disposable.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`...disposableLikes` | { dispose: () => any  }[] | Objects that have at least a `dispose`-function member. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

Returns a new disposable which, upon dispose, will
dispose all provided disposables.
