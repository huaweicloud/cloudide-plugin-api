[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugAdapterDescriptorFactory

# Interface: DebugAdapterDescriptorFactory

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugAdapterDescriptorFactory

## Table of contents

### Methods

- [createDebugAdapterDescriptor](cloudide_plugin_.DebugAdapterDescriptorFactory.md#createdebugadapterdescriptor)

## Methods

### createDebugAdapterDescriptor

▸ **createDebugAdapterDescriptor**(`session`, `executable`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DebugAdapterDescriptor`](../modules/_cloudide_plugin_.md#debugadapterdescriptor)\>

'createDebugAdapterDescriptor' is called at the start of a debug session to provide details about the debug adapter to use.
These details must be returned as objects of type [DebugAdapterDescriptor](#DebugAdapterDescriptor).
Currently two types of debug adapters are supported:
- a debug adapter executable is specified as a command path and arguments (see [DebugAdapterExecutable](#DebugAdapterExecutable)),
- a debug adapter server reachable via a communication port (see [DebugAdapterServer](#DebugAdapterServer)).
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
| `session` | [`DebugSession`](cloudide_plugin_.DebugSession.md) | The [debug session](#DebugSession) for which the debug adapter will be used. |
| `executable` | `undefined` \| [`DebugAdapterExecutable`](../classes/cloudide_plugin_.DebugAdapterExecutable.md) | The debug adapter's executable information as specified in the package.json (or undefined if no such information exists). |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DebugAdapterDescriptor`](../modules/_cloudide_plugin_.md#debugadapterdescriptor)\>

a [debug adapter descriptor](#DebugAdapterDescriptor) or undefined.

#### Defined in

[index.d.ts:9902](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9902)
