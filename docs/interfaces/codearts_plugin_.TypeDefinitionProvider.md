[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TypeDefinitionProvider

# Interface: TypeDefinitionProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).TypeDefinitionProvider

## Table of contents

### Methods

- [provideTypeDefinition](codearts_plugin_.TypeDefinitionProvider.md#providetypedefinition)

## Methods

### provideTypeDefinition

▸ **provideTypeDefinition**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Definition`](../modules/_codearts_plugin_.md#definition) \| [`LocationLink`](codearts_plugin_.LocationLink.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Definition`](../modules/_codearts_plugin_.md#definition) \| [`LocationLink`](codearts_plugin_.LocationLink.md)[]\>

#### Defined in

[index.d.ts:2707](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L2707)
