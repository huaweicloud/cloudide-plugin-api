[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TreeDataProvider

# Interface: TreeDataProvider<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TreeDataProvider

A data provider that provides tree data

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Properties

- [onDidChangeTreeData](cloudide_plugin_.TreeDataProvider.md#ondidchangetreedata)

### Methods

- [getChildren](cloudide_plugin_.TreeDataProvider.md#getchildren)
- [getParent](cloudide_plugin_.TreeDataProvider.md#getparent)
- [getTreeItem](cloudide_plugin_.TreeDataProvider.md#gettreeitem)

## Properties

### onDidChangeTreeData

• `Optional` **onDidChangeTreeData**: [`Event`](cloudide_plugin_.Event.md)<`undefined` \| ``null`` \| `T`\>

An optional event to signal that an element or root has changed.
This will trigger the view to update the changed element/root and its children recursively (if shown).
To signal that root has changed, do not pass any argument or pass `undefined` or `null`.

#### Defined in

[index.d.ts:5275](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5275)

## Methods

### getChildren

▸ **getChildren**(`element?`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

Get the children of `element` or root if no element is passed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element?` | `T` | The element from which the provider gets children. Can be `undefined`. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

Children of `element` or root if no element is passed.

#### Defined in

[index.d.ts:5291](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5291)

___

### getParent

▸ `Optional` **getParent**(`element`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

Optional method to return the parent of `element`.
Return `null` or `undefined` if `element` is a child of root.

**NOTE:** This method should be implemented in order to access [reveal](#TreeView.reveal) API.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `T` | The element for which the parent has to be returned. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

Parent of `element`.

#### Defined in

[index.d.ts:5302](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5302)

___

### getTreeItem

▸ **getTreeItem**(`element`): [`TreeItem`](../classes/cloudide_plugin_.TreeItem.md) \| `PromiseLike`<[`TreeItem`](../classes/cloudide_plugin_.TreeItem.md)\>

Get [TreeItem](#TreeItem) representation of the `element`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `T` | The element for which [TreeItem](#TreeItem) representation is asked for. |

#### Returns

[`TreeItem`](../classes/cloudide_plugin_.TreeItem.md) \| `PromiseLike`<[`TreeItem`](../classes/cloudide_plugin_.TreeItem.md)\>

[TreeItem](#TreeItem) representation of the element

#### Defined in

[index.d.ts:5283](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5283)
