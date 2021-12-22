**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TreeDataProvider

# Interface: TreeDataProvider\<T>

A data provider that provides tree data

## Type parameters

Name |
------ |
`T` |

## Hierarchy

* **TreeDataProvider**

## Index

### Properties

* [onDidChangeTreeData](_index_d_._plugin_.treedataprovider.md#ondidchangetreedata)

### Methods

* [getChildren](_index_d_._plugin_.treedataprovider.md#getchildren)
* [getParent](_index_d_._plugin_.treedataprovider.md#getparent)
* [getTreeItem](_index_d_._plugin_.treedataprovider.md#gettreeitem)
* [resolveTreeItem](_index_d_._plugin_.treedataprovider.md#resolvetreeitem)

## Properties

### onDidChangeTreeData

• `Optional` **onDidChangeTreeData**: [Event](_index_d_._plugin_.event.md)\<T \| undefined \| null \| void>

*Defined in [index.d.ts:9151](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9151)*

An optional event to signal that an element or root has changed.
This will trigger the view to update the changed element/root and its children recursively (if shown).
To signal that root has changed, do not pass any argument or pass `undefined` or `null`.

## Methods

### getChildren

▸ **getChildren**(`element?`: T): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

*Defined in [index.d.ts:9167](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9167)*

Get the children of `element` or root if no element is passed.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`element?` | T | The element from which the provider gets children. Can be `undefined`. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

Children of `element` or root if no element is passed.

___

### getParent

▸ `Optional`**getParent**(`element`: T): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T>

*Defined in [index.d.ts:9178](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9178)*

Optional method to return the parent of `element`.
Return `null` or `undefined` if `element` is a child of root.

**NOTE:** This method should be implemented in order to access [reveal](#TreeView.reveal) API.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`element` | T | The element for which the parent has to be returned. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T>

Parent of `element`.

___

### getTreeItem

▸ **getTreeItem**(`element`: T): [TreeItem](../classes/_index_d_._plugin_.treeitem.md) \| [Thenable](_index_d_.thenable.md)\<[TreeItem](../classes/_index_d_._plugin_.treeitem.md)>

*Defined in [index.d.ts:9159](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9159)*

Get [TreeItem](#TreeItem) representation of the `element`

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`element` | T | The element for which [TreeItem](#TreeItem) representation is asked for. |

**Returns:** [TreeItem](../classes/_index_d_._plugin_.treeitem.md) \| [Thenable](_index_d_.thenable.md)\<[TreeItem](../classes/_index_d_._plugin_.treeitem.md)>

(#TreeItem) representation of the element

___

### resolveTreeItem

▸ `Optional`**resolveTreeItem**(`item`: [TreeItem](../classes/_index_d_._plugin_.treeitem.md), `element`: T, `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[TreeItem](../classes/_index_d_._plugin_.treeitem.md)>

*Defined in [index.d.ts:9201](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9201)*

Called on hover to resolve the [TreeItem](#TreeItem.tooltip) property if it is undefined.
Called on tree item click/open to resolve the [TreeItem](#TreeItem.command) property if it is undefined.
Only properties that were undefined can be resolved in `resolveTreeItem`.
Functionality may be expanded later to include being called to resolve other missing
properties on selection and/or on open.

Will only ever be called once per TreeItem.

onDidChangeTreeData should not be triggered from within resolveTreeItem.

*Note* that this function is called when tree items are already showing in the UI.
Because of that, no property that changes the presentation (label, description, etc.)
can be changed.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`item` | [TreeItem](../classes/_index_d_._plugin_.treeitem.md) | Undefined properties of `item` should be set then `item` should be returned. |
`element` | T | The object associated with the TreeItem. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[TreeItem](../classes/_index_d_._plugin_.treeitem.md)>

The resolved tree item or a thenable that resolves to such. It is OK to return the given
`item`. When no result is returned, the given `item` will be used.
