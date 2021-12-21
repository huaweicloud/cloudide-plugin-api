**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugConfigurationProviderTriggerKind

# Enumeration: DebugConfigurationProviderTriggerKind

A DebugConfigurationProviderTriggerKind specifies when the `provideDebugConfigurations` method of a `DebugConfigurationProvider` is triggered.
Currently there are two situations: to provide the initial debug configurations for a newly created launch.json or
to provide dynamically generated debug configurations when the user asks for them through the UI (e.g. via the "Select and Start Debugging" command).
A trigger kind is used when registering a `DebugConfigurationProvider` with #debug.registerDebugConfigurationProvider.

## Index

### Enumeration members

* [Dynamic](_index_d_._plugin_.debugconfigurationprovidertriggerkind.md#dynamic)
* [Initial](_index_d_._plugin_.debugconfigurationprovidertriggerkind.md#initial)

## Enumeration members

### Dynamic

•  **Dynamic**:  = 2

*Defined in [index.d.ts:11965](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11965)*

`DebugConfigurationProvider.provideDebugConfigurations` is called to provide dynamically generated debug configurations when the user asks for them through the UI (e.g. via the "Select and Start Debugging" command).

___

### Initial

•  **Initial**:  = 1

*Defined in [index.d.ts:11961](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11961)*

	`DebugConfigurationProvider.provideDebugConfigurations` is called to provide the initial debug configurations for a newly created launch.json.
