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

## Properties

### onDidChangeTreeData

• `Optional` **onDidChangeTreeData**: [Event](_index_d_._plugin_.event.md)\<T \| undefined \| null \| void>

*Defined in [index.d.ts:7940](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7940)*

An optional event to signal that an element or root has changed.
This will trigger the view to update the changed element/root and its children recursively (if shown).
To signal that root has changed, do not pass any argument or pass `undefined` or `null`.

## Methods

### getChildren

▸ **getChildren**(`element?`: T): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

*Defined in [index.d.ts:7956](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7956)*

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

*Defined in [index.d.ts:7967](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7967)*

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

*Defined in [index.d.ts:7948](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7948)*

Get [TreeItem](#TreeItem) representation of the `element`

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`element` | T | The element for which [TreeItem](#TreeItem) representation is asked for. |

**Returns:** [TreeItem](../classes/_index_d_._plugin_.treeitem.md) \| [Thenable](_index_d_.thenable.md)\<[TreeItem](../classes/_index_d_._plugin_.treeitem.md)>

(#TreeItem) representation of the element
