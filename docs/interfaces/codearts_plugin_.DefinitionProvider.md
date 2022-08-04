[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DefinitionProvider

# Interface: DefinitionProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DefinitionProvider

## Table of contents

### Methods

- [provideDefinition](codearts_plugin_.DefinitionProvider.md#providedefinition)

## Methods

### provideDefinition

▸ **provideDefinition**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Definition`](../modules/_codearts_plugin_.md#definition) \| [`LocationLink`](codearts_plugin_.LocationLink.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Definition`](../modules/_codearts_plugin_.md#definition) \| [`LocationLink`](codearts_plugin_.LocationLink.md)[]\>

#### Defined in

[index.d.ts:2671](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L2671)
