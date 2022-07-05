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

[index.d.ts:10250](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L10250)

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

[index.d.ts:10266](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L10266)

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

[index.d.ts:10277](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L10277)

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

[index.d.ts:10258](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L10258)

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

[index.d.ts:10300](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L10300)
