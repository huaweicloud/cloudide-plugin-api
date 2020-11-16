**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugAdapterTrackerFactory

# Interface: DebugAdapterTrackerFactory

## Hierarchy

* **DebugAdapterTrackerFactory**

## Index

### Methods

* [createDebugAdapterTracker](_index_d_._plugin_.debugadaptertrackerfactory.md#createdebugadaptertracker)

## Methods

### createDebugAdapterTracker

▸ **createDebugAdapterTracker**(`session`: [DebugSession](_index_d_._plugin_.debugsession.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DebugAdapterTracker](_index_d_._plugin_.debugadaptertracker.md)>

*Defined in [index.d.ts:10386](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10386)*

The method 'createDebugAdapterTracker' is called at the start of a debug session in order
to return a "tracker" object that provides read-access to the communication between VS Code and a debug adapter.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`session` | [DebugSession](_index_d_._plugin_.debugsession.md) | The [debug session](#DebugSession) for which the debug adapter tracker will be used. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DebugAdapterTracker](_index_d_._plugin_.debugadaptertracker.md)>

A [debug adapter tracker](#DebugAdapterTracker) or undefined.
