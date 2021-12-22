**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugConfigurationProvider

# Interface: DebugConfigurationProvider

A debug configuration provider allows to add debug configurations to the debug service
and to resolve launch configurations before they are used to start a debug session.
A debug configuration provider is registered via #debug.registerDebugConfigurationProvider.

## Hierarchy

* **DebugConfigurationProvider**

## Index

### Methods

* [provideDebugConfigurations](_index_d_._plugin_.debugconfigurationprovider.md#providedebugconfigurations)
* [resolveDebugConfiguration](_index_d_._plugin_.debugconfigurationprovider.md#resolvedebugconfiguration)
* [resolveDebugConfigurationWithSubstitutedVariables](_index_d_._plugin_.debugconfigurationprovider.md#resolvedebugconfigurationwithsubstitutedvariables)

## Methods

### provideDebugConfigurations

▸ `Optional`**provideDebugConfigurations**(`folder`: [WorkspaceFolder](_index_d_._plugin_.workspacefolder.md) \| undefined, `token?`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DebugConfiguration](_index_d_._plugin_.debugconfiguration.md)[]>

*Defined in [index.d.ts:11623](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11623)*

Provides [debug configuration](#DebugConfiguration) to the debug service. If more than one debug configuration provider is
registered for the same type, debug configurations are concatenated in arbitrary order.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`folder` | [WorkspaceFolder](_index_d_._plugin_.workspacefolder.md) \| undefined | The workspace folder for which the configurations are used or `undefined` for a folderless setup. |
`token?` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DebugConfiguration](_index_d_._plugin_.debugconfiguration.md)[]>

An array of [debug configurations](#DebugConfiguration).

___

### resolveDebugConfiguration

▸ `Optional`**resolveDebugConfiguration**(`folder`: [WorkspaceFolder](_index_d_._plugin_.workspacefolder.md) \| undefined, `debugConfiguration`: [DebugConfiguration](_index_d_._plugin_.debugconfiguration.md), `token?`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DebugConfiguration](_index_d_._plugin_.debugconfiguration.md)>

*Defined in [index.d.ts:11637](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11637)*

Resolves a [debug configuration](#DebugConfiguration) by filling in missing values or by adding/changing/removing attributes.
If more than one debug configuration provider is registered for the same type, the resolveDebugConfiguration calls are chained
in arbitrary order and the initial debug configuration is piped through the chain.
Returning the value 'undefined' prevents the debug session from starting.
Returning the value 'null' prevents the debug session from starting and opens the underlying debug configuration instead.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`folder` | [WorkspaceFolder](_index_d_._plugin_.workspacefolder.md) \| undefined | The workspace folder from which the configuration originates from or `undefined` for a folderless setup. |
`debugConfiguration` | [DebugConfiguration](_index_d_._plugin_.debugconfiguration.md) | The [debug configuration](#DebugConfiguration) to resolve. |
`token?` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DebugConfiguration](_index_d_._plugin_.debugconfiguration.md)>

The resolved debug configuration or undefined or null.

___

### resolveDebugConfigurationWithSubstitutedVariables

▸ `Optional`**resolveDebugConfigurationWithSubstitutedVariables**(`folder`: [WorkspaceFolder](_index_d_._plugin_.workspacefolder.md) \| undefined, `debugConfiguration`: [DebugConfiguration](_index_d_._plugin_.debugconfiguration.md), `token?`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DebugConfiguration](_index_d_._plugin_.debugconfiguration.md)>

*Defined in [index.d.ts:11652](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11652)*

This hook is directly called after 'resolveDebugConfiguration' but with all variables substituted.
It can be used to resolve or verify a [debug configuration](#DebugConfiguration) by filling in missing values or by adding/changing/removing attributes.
If more than one debug configuration provider is registered for the same type, the 'resolveDebugConfigurationWithSubstitutedVariables' calls are chained
in arbitrary order and the initial debug configuration is piped through the chain.
Returning the value 'undefined' prevents the debug session from starting.
Returning the value 'null' prevents the debug session from starting and opens the underlying debug configuration instead.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`folder` | [WorkspaceFolder](_index_d_._plugin_.workspacefolder.md) \| undefined | The workspace folder from which the configuration originates from or `undefined` for a folderless setup. |
`debugConfiguration` | [DebugConfiguration](_index_d_._plugin_.debugconfiguration.md) | The [debug configuration](#DebugConfiguration) to resolve. |
`token?` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DebugConfiguration](_index_d_._plugin_.debugconfiguration.md)>

The resolved debug configuration or undefined or null.
