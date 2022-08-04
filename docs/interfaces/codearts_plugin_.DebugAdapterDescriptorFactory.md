[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugAdapterDescriptorFactory

# Interface: DebugAdapterDescriptorFactory

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugAdapterDescriptorFactory

## Table of contents

### Methods

- [createDebugAdapterDescriptor](codearts_plugin_.DebugAdapterDescriptorFactory.md#createdebugadapterdescriptor)

## Methods

### createDebugAdapterDescriptor

▸ **createDebugAdapterDescriptor**(`session`, `executable`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugAdapterDescriptor`](../modules/_codearts_plugin_.md#debugadapterdescriptor)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `session` | [`DebugSession`](codearts_plugin_.DebugSession.md) |  |
| `executable` | `undefined` \| [`DebugAdapterExecutable`](../classes/codearts_plugin_.DebugAdapterExecutable.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugAdapterDescriptor`](../modules/_codearts_plugin_.md#debugadapterdescriptor)\>

#### Defined in

[index.d.ts:14341](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14341)
