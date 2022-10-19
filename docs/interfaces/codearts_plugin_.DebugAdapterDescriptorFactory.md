[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugAdapterDescriptorFactory

# Interface: DebugAdapterDescriptorFactory

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugAdapterDescriptorFactory

## Table of contents

### Methods

- [createDebugAdapterDescriptor](codearts_plugin_.DebugAdapterDescriptorFactory.md#createdebugadapterdescriptor)

## Methods

### createDebugAdapterDescriptor

▸ **createDebugAdapterDescriptor**(`session`, `executable`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugAdapterDescriptor`](../modules/_codearts_plugin_.md#debugadapterdescriptor)\>

'createDebugAdapterDescriptor' is called at the start of a debug session to provide details about the debug adapter to use.
These details must be returned as objects of type [DebugAdapterDescriptor](../modules/_codearts_plugin_.md#debugadapterdescriptor).
Currently two types of debug adapters are supported:
- a debug adapter executable is specified as a command path and arguments (see [DebugAdapterExecutable](../classes/codearts_plugin_.DebugAdapterExecutable.md)),
- a debug adapter server reachable via a communication port (see [DebugAdapterServer](../classes/codearts_plugin_.DebugAdapterServer.md)).
If the method is not implemented the default behavior is this:
  createDebugAdapter(session: DebugSession, executable: DebugAdapterExecutable) {
     if (typeof session.configuration.debugServer === 'number') {
        return new DebugAdapterServer(session.configuration.debugServer);
     }
     return executable;
  }

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `session` | [`DebugSession`](codearts_plugin_.DebugSession.md) | The [debug session](codearts_plugin_.DebugSession.md) for which the debug adapter will be used. |
| `executable` | `undefined` \| [`DebugAdapterExecutable`](../classes/codearts_plugin_.DebugAdapterExecutable.md) | The debug adapter's executable information as specified in the package.json (or undefined if no such information exists). |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugAdapterDescriptor`](../modules/_codearts_plugin_.md#debugadapterdescriptor)\>

a [debug adapter descriptor](../modules/_codearts_plugin_.md#debugadapterdescriptor) or undefined.

#### Defined in

[index.d.ts:14569](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14569)
