[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TreeDataProvider

# Interface: TreeDataProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).TreeDataProvider

A data provider that provides tree data

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

An optional event to signal that an element or root has changed.
This will trigger the view to update the changed element/root and its children recursively (if shown).
To signal that root has changed, do not pass any argument or pass `undefined` or `null`.

#### Defined in

[index.d.ts:10766](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10766)

## Methods

### getChildren

▸ **getChildren**(`element?`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

Get the children of `element` or root if no element is passed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element?` | `T` | The element from which the provider gets children. Can be `undefined`. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

Children of `element` or root if no element is passed.

#### Defined in

[index.d.ts:10782](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10782)

___

### getParent

▸ `Optional` **getParent**(`element`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

Optional method to return the parent of `element`.
Return `null` or `undefined` if `element` is a child of root.

**NOTE:** This method should be implemented in order to access [reveal](codearts_plugin_.TreeView.md#reveal) API.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `T` | The element for which the parent has to be returned. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

Parent of `element`.

#### Defined in

[index.d.ts:10793](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10793)

___

### getTreeItem

▸ **getTreeItem**(`element`): [`TreeItem`](../classes/codearts_plugin_.TreeItem.md) \| [`Thenable`](Thenable.md)<[`TreeItem`](../classes/codearts_plugin_.TreeItem.md)\>

Get [TreeItem](../classes/codearts_plugin_.TreeItem.md) representation of the `element`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `T` | The element for which [TreeItem](../classes/codearts_plugin_.TreeItem.md) representation is asked for. |

#### Returns

[`TreeItem`](../classes/codearts_plugin_.TreeItem.md) \| [`Thenable`](Thenable.md)<[`TreeItem`](../classes/codearts_plugin_.TreeItem.md)\>

TreeItem representation of the element.

#### Defined in

[index.d.ts:10774](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10774)

___

### resolveTreeItem

▸ `Optional` **resolveTreeItem**(`item`, `element`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TreeItem`](../classes/codearts_plugin_.TreeItem.md)\>

Called on hover to resolve the [TreeItem](../classes/codearts_plugin_.TreeItem.md#tooltip) property if it is undefined.
Called on tree item click/open to resolve the [TreeItem](../classes/codearts_plugin_.TreeItem.md#command) property if it is undefined.
Only properties that were undefined can be resolved in `resolveTreeItem`.
Functionality may be expanded later to include being called to resolve other missing
properties on selection and/or on open.

Will only ever be called once per TreeItem.

onDidChangeTreeData should not be triggered from within resolveTreeItem.

*Note* that this function is called when tree items are already showing in the UI.
Because of that, no property that changes the presentation (label, description, etc.)
can be changed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`TreeItem`](../classes/codearts_plugin_.TreeItem.md) | Undefined properties of `item` should be set then `item` should be returned. |
| `element` | `T` | The object associated with the TreeItem. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TreeItem`](../classes/codearts_plugin_.TreeItem.md)\>

The resolved tree item or a thenable that resolves to such. It is OK to return the given
`item`. When no result is returned, the given `item` will be used.

#### Defined in

[index.d.ts:10816](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10816)
