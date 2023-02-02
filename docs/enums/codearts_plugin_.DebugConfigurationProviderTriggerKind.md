[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugConfigurationProviderTriggerKind

# Enumeration: DebugConfigurationProviderTriggerKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugConfigurationProviderTriggerKind

A DebugConfigurationProviderTriggerKind specifies when the `provideDebugConfigurations` method of a `DebugConfigurationProvider` is triggered.
Currently there are two situations: to provide the initial debug configurations for a newly created launch.json or
to provide dynamically generated debug configurations when the user asks for them through the UI (e.g. via the "Select and Start Debugging" command).
A trigger kind is used when registering a `DebugConfigurationProvider` with [registerDebugConfigurationProvider](../modules/codearts_plugin_.debug.md#registerdebugconfigurationprovider).

## Table of contents

### Enumeration Members

- [Dynamic](codearts_plugin_.DebugConfigurationProviderTriggerKind.md#dynamic)
- [Initial](codearts_plugin_.DebugConfigurationProviderTriggerKind.md#initial)

## Enumeration Members

### Dynamic

• **Dynamic** = ``2``

`DebugConfigurationProvider.provideDebugConfigurations` is called to provide dynamically generated debug configurations when the user asks for them through the UI (e.g. via the "Select and Start Debugging" command).

#### Defined in

[index.d.ts:15337](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15337)

___

### Initial

• **Initial** = ``1``

`DebugConfigurationProvider.provideDebugConfigurations` is called to provide the initial debug configurations for a newly created launch.json.

#### Defined in

[index.d.ts:15333](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15333)
