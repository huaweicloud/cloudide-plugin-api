[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugConfigurationProvider

# Interface: DebugConfigurationProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugConfigurationProvider

## Table of contents

### Methods

- [provideDebugConfigurations](codearts_plugin_.DebugConfigurationProvider.md#providedebugconfigurations)
- [resolveDebugConfiguration](codearts_plugin_.DebugConfigurationProvider.md#resolvedebugconfiguration)
- [resolveDebugConfigurationWithSubstitutedVariables](codearts_plugin_.DebugConfigurationProvider.md#resolvedebugconfigurationwithsubstitutedvariables)

## Methods

### provideDebugConfigurations

▸ `Optional` **provideDebugConfigurations**(`folder`, `token?`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](codearts_plugin_.WorkspaceFolder.md) |  |
| `token?` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)[]\>

#### Defined in

[index.d.ts:14141](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L14141)

___

### resolveDebugConfiguration

▸ `Optional` **resolveDebugConfiguration**(`folder`, `debugConfiguration`, `token?`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](codearts_plugin_.WorkspaceFolder.md) |  |
| `debugConfiguration` | [`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md) |  |
| `token?` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)\>

#### Defined in

[index.d.ts:14155](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L14155)

___

### resolveDebugConfigurationWithSubstitutedVariables

▸ `Optional` **resolveDebugConfigurationWithSubstitutedVariables**(`folder`, `debugConfiguration`, `token?`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](codearts_plugin_.WorkspaceFolder.md) |  |
| `debugConfiguration` | [`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md) |  |
| `token?` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)\>

#### Defined in

[index.d.ts:14170](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L14170)
