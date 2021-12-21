**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugAdapterDescriptorFactory

# Interface: DebugAdapterDescriptorFactory

## Hierarchy

* **DebugAdapterDescriptorFactory**

## Index

### Methods

* [createDebugAdapterDescriptor](_index_d_._plugin_.debugadapterdescriptorfactory.md#createdebugadapterdescriptor)

## Methods

### createDebugAdapterDescriptor

▸ **createDebugAdapterDescriptor**(`session`: [DebugSession](_index_d_._plugin_.debugsession.md), `executable`: [DebugAdapterExecutable](../classes/_index_d_._plugin_.debugadapterexecutable.md) \| undefined): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DebugAdapterDescriptor](../modules/_index_d_._plugin_.md#debugadapterdescriptor)>

*Defined in [index.d.ts:11761](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11761)*

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

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`session` | [DebugSession](_index_d_._plugin_.debugsession.md) | The [debug session](#DebugSession) for which the debug adapter will be used. |
`executable` | [DebugAdapterExecutable](../classes/_index_d_._plugin_.debugadapterexecutable.md) \| undefined | The debug adapter's executable information as specified in the package.json (or undefined if no such information exists). |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DebugAdapterDescriptor](../modules/_index_d_._plugin_.md#debugadapterdescriptor)>

a [debug adapter descriptor](#DebugAdapterDescriptor) or undefined.
