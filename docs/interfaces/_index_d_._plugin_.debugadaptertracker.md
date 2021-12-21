**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugAdapterTracker

# Interface: DebugAdapterTracker

A Debug Adapter Tracker is a means to track the communication between VS Code and a Debug Adapter.

## Hierarchy

* **DebugAdapterTracker**

## Index

### Methods

* [onDidSendMessage](_index_d_._plugin_.debugadaptertracker.md#ondidsendmessage)
* [onError](_index_d_._plugin_.debugadaptertracker.md#onerror)
* [onExit](_index_d_._plugin_.debugadaptertracker.md#onexit)
* [onWillReceiveMessage](_index_d_._plugin_.debugadaptertracker.md#onwillreceivemessage)
* [onWillStartSession](_index_d_._plugin_.debugadaptertracker.md#onwillstartsession)
* [onWillStopSession](_index_d_._plugin_.debugadaptertracker.md#onwillstopsession)

## Methods

### onDidSendMessage

▸ `Optional`**onDidSendMessage**(`message`: any): void

*Defined in [index.d.ts:11779](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11779)*

The debug adapter has sent a Debug Adapter Protocol message to VS Code.

#### Parameters:

Name | Type |
------ | ------ |
`message` | any |

**Returns:** void

___

### onError

▸ `Optional`**onError**(`error`: [Error](../classes/_index_d_._plugin_.cancellationerror.md#error)): void

*Defined in [index.d.ts:11787](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11787)*

An error with the debug adapter has occurred.

#### Parameters:

Name | Type |
------ | ------ |
`error` | [Error](../classes/_index_d_._plugin_.cancellationerror.md#error) |

**Returns:** void

___

### onExit

▸ `Optional`**onExit**(`code`: number \| undefined, `signal`: string \| undefined): void

*Defined in [index.d.ts:11791](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11791)*

The debug adapter has exited with the given exit code or signal.

#### Parameters:

Name | Type |
------ | ------ |
`code` | number \| undefined |
`signal` | string \| undefined |

**Returns:** void

___

### onWillReceiveMessage

▸ `Optional`**onWillReceiveMessage**(`message`: any): void

*Defined in [index.d.ts:11775](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11775)*

The debug adapter is about to receive a Debug Adapter Protocol message from VS Code.

#### Parameters:

Name | Type |
------ | ------ |
`message` | any |

**Returns:** void

___

### onWillStartSession

▸ `Optional`**onWillStartSession**(): void

*Defined in [index.d.ts:11771](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11771)*

A session with the debug adapter is about to be started.

**Returns:** void

___

### onWillStopSession

▸ `Optional`**onWillStopSession**(): void

*Defined in [index.d.ts:11783](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11783)*

The debug adapter session is about to be stopped.

**Returns:** void
