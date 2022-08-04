[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TreeDataProvider

# Interface: TreeDataProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).TreeDataProvider

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Properties

- [onDidChangeTreeData](codearts_plugin_.TreeDataProvider.md#ondidchangetreedata)

### Methods

- [getChildren](codearts_plugin_.TreeDataProvider.md#getchildren)
- [getParent](codearts_plugin_.TreeDataProvider.md#getparent)
- [getTreeItem](codearts_plugin_.TreeDataProvider.md#gettreeitem)
- [resolveTreeItem](codearts_plugin_.TreeDataProvider.md#resolvetreeitem)

## Properties

### onDidChangeTreeData

• `Optional` **onDidChangeTreeData**: [`Event`](codearts_plugin_.Event.md)<`undefined` \| ``null`` \| `void` \| `T` \| `T`[]\>

#### Defined in

[index.d.ts:10280](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10280)

## Methods

### getChildren

▸ **getChildren**(`element?`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element?` | `T` |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Defined in

[index.d.ts:10296](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10296)

___

### getParent

▸ `Optional` **getParent**(`element`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `T` |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Defined in

[index.d.ts:10307](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10307)

___

### getTreeItem

▸ **getTreeItem**(`element`): [`TreeItem`](../classes/codearts_plugin_.TreeItem.md) \| [`Thenable`](Thenable.md)<[`TreeItem`](../classes/codearts_plugin_.TreeItem.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `T` |  |

#### Returns

[`TreeItem`](../classes/codearts_plugin_.TreeItem.md) \| [`Thenable`](Thenable.md)<[`TreeItem`](../classes/codearts_plugin_.TreeItem.md)\>

#### Defined in

[index.d.ts:10288](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10288)

___

### resolveTreeItem

▸ `Optional` **resolveTreeItem**(`item`, `element`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TreeItem`](../classes/codearts_plugin_.TreeItem.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`TreeItem`](../classes/codearts_plugin_.TreeItem.md) |  |
| `element` | `T` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TreeItem`](../classes/codearts_plugin_.TreeItem.md)\>

#### Defined in

[index.d.ts:10330](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10330)
