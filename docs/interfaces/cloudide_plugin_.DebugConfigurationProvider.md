[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugConfigurationProvider

# Interface: DebugConfigurationProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugConfigurationProvider

A debug configuration provider allows to add the initial debug configurations to a newly created launch.json
and to resolve a launch configuration before it is used to start a new debug session.
A debug configuration provider is registered via #debug.registerDebugConfigurationProvider.

## Table of contents

### Methods

- [provideDebugConfigurations](cloudide_plugin_.DebugConfigurationProvider.md#providedebugconfigurations)
- [resolveDebugConfiguration](cloudide_plugin_.DebugConfigurationProvider.md#resolvedebugconfiguration)
- [resolveDebugConfigurationWithSubstitutedVariables](cloudide_plugin_.DebugConfigurationProvider.md#resolvedebugconfigurationwithsubstitutedvariables)

## Methods

### provideDebugConfigurations

▸ `Optional` **provideDebugConfigurations**(`folder`, `token?`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DebugConfiguration`](cloudide_plugin_.DebugConfiguration.md)[]\>

Provides initial [debug configuration](#DebugConfiguration). If more than one debug configuration provider is
registered for the same type, debug configurations are concatenated in arbitrary order.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](cloudide_plugin_.WorkspaceFolder.md) | The workspace folder for which the configurations are used or undefined for a folderless setup. |
| `token?` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DebugConfiguration`](cloudide_plugin_.DebugConfiguration.md)[]\>

An array of [debug configurations](cloudide_plugin_.DebugConfiguration.md).

#### Defined in

[index.d.ts:9691](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9691)

___

### resolveDebugConfiguration

▸ `Optional` **resolveDebugConfiguration**(`folder`, `debugConfiguration`, `token?`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DebugConfiguration`](cloudide_plugin_.DebugConfiguration.md)\>

Resolves a [debug configuration](#DebugConfiguration) by filling in missing values or by adding/changing/removing attributes.
If more than one debug configuration provider is registered for the same type, the resolveDebugConfiguration calls are chained
in arbitrary order and the initial debug configuration is piped through the chain.
Returning the value 'undefined' prevents the debug session from starting.
Returning the value 'null' prevents the debug session from starting and opens the underlying debug configuration instead.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](cloudide_plugin_.WorkspaceFolder.md) | The workspace folder from which the configuration originates from or undefined for a folderless setup. |
| `debugConfiguration` | [`DebugConfiguration`](cloudide_plugin_.DebugConfiguration.md) | The [debug configuration](#DebugConfiguration) to resolve. |
| `token?` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DebugConfiguration`](cloudide_plugin_.DebugConfiguration.md)\>

The resolved debug configuration or undefined or null.

#### Defined in

[index.d.ts:9705](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9705)

___

### resolveDebugConfigurationWithSubstitutedVariables

▸ `Optional` **resolveDebugConfigurationWithSubstitutedVariables**(`folder`, `debugConfiguration`, `token?`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DebugConfiguration`](cloudide_plugin_.DebugConfiguration.md)\>

This hook is directly called after 'resolveDebugConfiguration' but with all variables substituted.
It can be used to resolve or verify a [debug configuration](#DebugConfiguration) by filling in missing values or by adding/changing/removing attributes.
If more than one debug configuration provider is registered for the same type, the 'resolveDebugConfigurationWithSubstitutedVariables' calls are chained
in arbitrary order and the initial debug configuration is piped through the chain.
Returning the value 'undefined' prevents the debug session from starting.
Returning the value 'null' prevents the debug session from starting and opens the underlying debug configuration instead.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](cloudide_plugin_.WorkspaceFolder.md) | The workspace folder from which the configuration originates from or `undefined` for a folderless setup. |
| `debugConfiguration` | [`DebugConfiguration`](cloudide_plugin_.DebugConfiguration.md) | The [debug configuration](#DebugConfiguration) to resolve. |
| `token?` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`DebugConfiguration`](cloudide_plugin_.DebugConfiguration.md)\>

The resolved debug configuration or undefined or null.

#### Defined in

[index.d.ts:9720](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9720)
