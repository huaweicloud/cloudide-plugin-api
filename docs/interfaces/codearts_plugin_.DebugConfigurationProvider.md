[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugConfigurationProvider

# Interface: DebugConfigurationProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugConfigurationProvider

A debug configuration provider allows to add debug configurations to the debug service
and to resolve launch configurations before they are used to start a debug session.
A debug configuration provider is registered via [registerDebugConfigurationProvider](../modules/codearts_plugin_.debug.md#registerdebugconfigurationprovider).

## Table of contents

### Methods

- [provideDebugConfigurations](codearts_plugin_.DebugConfigurationProvider.md#providedebugconfigurations)
- [resolveDebugConfiguration](codearts_plugin_.DebugConfigurationProvider.md#resolvedebugconfiguration)
- [resolveDebugConfigurationWithSubstitutedVariables](codearts_plugin_.DebugConfigurationProvider.md#resolvedebugconfigurationwithsubstitutedvariables)

## Methods

### provideDebugConfigurations

▸ `Optional` **provideDebugConfigurations**(`folder`, `token?`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)[]\>

Provides [debug configuration](codearts_plugin_.DebugConfiguration.md) to the debug service. If more than one debug configuration provider is
registered for the same type, debug configurations are concatenated in arbitrary order.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](codearts_plugin_.WorkspaceFolder.md) | The workspace folder for which the configurations are used or `undefined` for a folderless setup. |
| `token?` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)[]\>

An array of [debug configurations](codearts_plugin_.DebugConfiguration.md).

#### Defined in

[index.d.ts:14956](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14956)

___

### resolveDebugConfiguration

▸ `Optional` **resolveDebugConfiguration**(`folder`, `debugConfiguration`, `token?`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)\>

Resolves a [debug configuration](codearts_plugin_.DebugConfiguration.md) by filling in missing values or by adding/changing/removing attributes.
If more than one debug configuration provider is registered for the same type, the resolveDebugConfiguration calls are chained
in arbitrary order and the initial debug configuration is piped through the chain.
Returning the value 'undefined' prevents the debug session from starting.
Returning the value 'null' prevents the debug session from starting and opens the underlying debug configuration instead.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](codearts_plugin_.WorkspaceFolder.md) | The workspace folder from which the configuration originates from or `undefined` for a folderless setup. |
| `debugConfiguration` | [`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md) | The [debug configuration](codearts_plugin_.DebugConfiguration.md) to resolve. |
| `token?` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)\>

The resolved debug configuration or undefined or null.

#### Defined in

[index.d.ts:14970](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14970)

___

### resolveDebugConfigurationWithSubstitutedVariables

▸ `Optional` **resolveDebugConfigurationWithSubstitutedVariables**(`folder`, `debugConfiguration`, `token?`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)\>

This hook is directly called after 'resolveDebugConfiguration' but with all variables substituted.
It can be used to resolve or verify a [debug configuration](codearts_plugin_.DebugConfiguration.md) by filling in missing values or by adding/changing/removing attributes.
If more than one debug configuration provider is registered for the same type, the 'resolveDebugConfigurationWithSubstitutedVariables' calls are chained
in arbitrary order and the initial debug configuration is piped through the chain.
Returning the value 'undefined' prevents the debug session from starting.
Returning the value 'null' prevents the debug session from starting and opens the underlying debug configuration instead.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](codearts_plugin_.WorkspaceFolder.md) | The workspace folder from which the configuration originates from or `undefined` for a folderless setup. |
| `debugConfiguration` | [`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md) | The [debug configuration](codearts_plugin_.DebugConfiguration.md) to resolve. |
| `token?` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)\>

The resolved debug configuration or undefined or null.

#### Defined in

[index.d.ts:14985](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14985)
