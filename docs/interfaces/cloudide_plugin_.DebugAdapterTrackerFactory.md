[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugAdapterTrackerFactory

# Interface: DebugAdapterTrackerFactory

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugAdapterTrackerFactory

## Table of contents

### Methods

- [createDebugAdapterTracker](cloudide_plugin_.DebugAdapterTrackerFactory.md#createdebugadaptertracker)

## Methods

### createDebugAdapterTracker

▸ **createDebugAdapterTracker**(`session`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DebugAdapterTracker`](cloudide_plugin_.DebugAdapterTracker.md)\>

The method 'createDebugAdapterTracker' is called at the start of a debug session in order
to return a "tracker" object that provides read-access to the communication between VS Code and a debug adapter.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `session` | [`DebugSession`](cloudide_plugin_.DebugSession.md) | The [debug session](#DebugSession) for which the debug adapter tracker will be used. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DebugAdapterTracker`](cloudide_plugin_.DebugAdapterTracker.md)\>

A [debug adapter tracker](#DebugAdapterTracker) or undefined.

#### Defined in

[index.d.ts:9761](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9761)
