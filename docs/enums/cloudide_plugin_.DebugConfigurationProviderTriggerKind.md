[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugConfigurationProviderTriggerKind

# Enumeration: DebugConfigurationProviderTriggerKind

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugConfigurationProviderTriggerKind

A DebugConfigurationProviderTriggerKind specifies when the `provideDebugConfigurations` method of a `DebugConfigurationProvider` should be called.
Currently there are two situations:
 (1) providing debug configurations to populate a newly created `launch.json`
 (2) providing dynamically generated configurations when the user asks for them through the UI (e.g. via the "Select and Start Debugging" command).
A trigger kind is used when registering a `DebugConfigurationProvider` with [registerDebugConfigurationProvider](../modules/cloudide_plugin_.debug.md#registerdebugconfigurationprovider).

## Table of contents

### Enumeration Members

- [Dynamic](cloudide_plugin_.DebugConfigurationProviderTriggerKind.md#dynamic)
- [Initial](cloudide_plugin_.DebugConfigurationProviderTriggerKind.md#initial)

## Enumeration Members

### Dynamic

• **Dynamic** = ``2``

`DebugConfigurationProvider.provideDebugConfigurations` is called to provide dynamically generated debug configurations when the user asks for them through the UI
(e.g. via the "Select and Start Debugging" command).

#### Defined in

[index.d.ts:10035](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10035)

___

### Initial

• **Initial** = ``1``

`DebugConfigurationProvider.provideDebugConfigurations` is called to provide the initial debug configurations for a newly created launch.json.

#### Defined in

[index.d.ts:10030](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10030)
