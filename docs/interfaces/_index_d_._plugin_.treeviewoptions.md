**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TreeViewOptions

# Interface: TreeViewOptions\<T>

Options for creating a [TreeView](#TreeView)

## Type parameters

Name |
------ |
`T` |

## Hierarchy

* **TreeViewOptions**

## Index

### Properties

* [canSelectMany](_index_d_._plugin_.treeviewoptions.md#canselectmany)
* [showCollapseAll](_index_d_._plugin_.treeviewoptions.md#showcollapseall)
* [treeDataProvider](_index_d_._plugin_.treeviewoptions.md#treedataprovider)

## Properties

### canSelectMany

• `Optional` **canSelectMany**: boolean

*Defined in [index.d.ts:7830](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7830)*

Whether the tree supports multi-select. When the tree supports multi-select and a command is executed from the tree,
the first argument to the command is the tree item that the command was executed on and the second argument is an
array containing all selected tree items.

___

### showCollapseAll

• `Optional` **showCollapseAll**: boolean

*Defined in [index.d.ts:7823](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7823)*

Whether to show collapse all action or not.

___

### treeDataProvider

•  **treeDataProvider**: [TreeDataProvider](_index_d_._plugin_.treedataprovider.md)\<T>

*Defined in [index.d.ts:7818](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7818)*

A data provider that provides tree data.
