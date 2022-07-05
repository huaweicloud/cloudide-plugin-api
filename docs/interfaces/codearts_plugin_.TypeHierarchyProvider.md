[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TypeHierarchyProvider

# Interface: TypeHierarchyProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).TypeHierarchyProvider

## Table of contents

### Methods

- [prepareTypeHierarchy](codearts_plugin_.TypeHierarchyProvider.md#preparetypehierarchy)
- [provideTypeHierarchySubtypes](codearts_plugin_.TypeHierarchyProvider.md#providetypehierarchysubtypes)
- [provideTypeHierarchySupertypes](codearts_plugin_.TypeHierarchyProvider.md#providetypehierarchysupertypes)

## Methods

### prepareTypeHierarchy

▸ **prepareTypeHierarchy**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md) \| [`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md) \| [`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

#### Defined in

[index.d.ts:5348](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L5348)

___

### provideTypeHierarchySubtypes

▸ **provideTypeHierarchySubtypes**(`item`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

#### Defined in

[index.d.ts:5372](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L5372)

___

### provideTypeHierarchySupertypes

▸ **provideTypeHierarchySupertypes**(`item`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

#### Defined in

[index.d.ts:5360](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L5360)
