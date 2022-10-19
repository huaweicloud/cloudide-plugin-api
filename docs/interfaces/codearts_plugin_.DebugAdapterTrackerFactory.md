[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugAdapterTrackerFactory

# Interface: DebugAdapterTrackerFactory

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugAdapterTrackerFactory

## Table of contents

### Methods

- [createDebugAdapterTracker](codearts_plugin_.DebugAdapterTrackerFactory.md#createdebugadaptertracker)

## Methods

### createDebugAdapterTracker

▸ **createDebugAdapterTracker**(`session`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugAdapterTracker`](codearts_plugin_.DebugAdapterTracker.md)\>

The method 'createDebugAdapterTracker' is called at the start of a debug session in order
to return a "tracker" object that provides read-access to the communication between the editor and a debug adapter.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `session` | [`DebugSession`](codearts_plugin_.DebugSession.md) | The [debug session](codearts_plugin_.DebugSession.md) for which the debug adapter tracker will be used. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugAdapterTracker`](codearts_plugin_.DebugAdapterTracker.md)\>

A [debug adapter tracker](codearts_plugin_.DebugAdapterTracker.md) or undefined.

#### Defined in

[index.d.ts:14610](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14610)
