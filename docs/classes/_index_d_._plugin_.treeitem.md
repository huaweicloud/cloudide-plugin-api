**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TreeItem

# Class: TreeItem

## Hierarchy

* **TreeItem**

## Index

### Constructors

* [constructor](_index_d_._plugin_.treeitem.md#constructor)

### Properties

* [collapsibleState](_index_d_._plugin_.treeitem.md#collapsiblestate)
* [command](_index_d_._plugin_.treeitem.md#command)
* [contextValue](_index_d_._plugin_.treeitem.md#contextvalue)
* [description](_index_d_._plugin_.treeitem.md#description)
* [iconPath](_index_d_._plugin_.treeitem.md#iconpath)
* [id](_index_d_._plugin_.treeitem.md#id)
* [label](_index_d_._plugin_.treeitem.md#label)
* [resourceUri](_index_d_._plugin_.treeitem.md#resourceuri)
* [tooltip](_index_d_._plugin_.treeitem.md#tooltip)

## Constructors

### constructor

\+ **new TreeItem**(`label`: string, `collapsibleState?`: [TreeItemCollapsibleState](../enums/_index_d_._plugin_.treeitemcollapsiblestate.md)): [TreeItem](_index_d_._plugin_.treeitem.md)

*Defined in [index.d.ts:8037](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8037)*

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`label` | string | A human-readable string describing this item |
`collapsibleState?` | [TreeItemCollapsibleState](../enums/_index_d_._plugin_.treeitemcollapsiblestate.md) | (#TreeItemCollapsibleState) of the tree item. Default is [TreeItemCollapsibleState.None](#TreeItemCollapsibleState.None)  |

**Returns:** [TreeItem](_index_d_._plugin_.treeitem.md)

\+ **new TreeItem**(`resourceUri`: [Uri](_index_d_._plugin_.uri.md), `collapsibleState?`: [TreeItemCollapsibleState](../enums/_index_d_._plugin_.treeitemcollapsiblestate.md)): [TreeItem](_index_d_._plugin_.treeitem.md)

*Defined in [index.d.ts:8043](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8043)*

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`resourceUri` | [Uri](_index_d_._plugin_.uri.md) | The [uri](#Uri) of the resource representing this item. |
`collapsibleState?` | [TreeItemCollapsibleState](../enums/_index_d_._plugin_.treeitemcollapsiblestate.md) | (#TreeItemCollapsibleState) of the tree item. Default is [TreeItemCollapsibleState.None](#TreeItemCollapsibleState.None)  |

**Returns:** [TreeItem](_index_d_._plugin_.treeitem.md)

## Properties

### collapsibleState

• `Optional` **collapsibleState**: [TreeItemCollapsibleState](../enums/_index_d_._plugin_.treeitemcollapsiblestate.md)

*Defined in [index.d.ts:8017](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8017)*

[TreeItemCollapsibleState](#TreeItemCollapsibleState) of the tree item.

___

### command

• `Optional` **command**: [Command](../interfaces/_index_d_._plugin_.command.md)

*Defined in [index.d.ts:8012](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8012)*

The [command](#Command) that should be executed when the tree item is selected.

___

### contextValue

• `Optional` **contextValue**: string

*Defined in [index.d.ts:8037](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8037)*

Context value of the tree item. This can be used to contribute item specific actions in the tree.
For example, a tree item is given a context value as `folder`. When contributing actions to `view/item/context`
using `menus` extension point, you can specify context value for key `viewItem` in `when` expression like `viewItem == folder`.
```
	"contributes": {
		"menus": {
			"view/item/context": [
				{
					"command": "extension.deleteFolder",
					"when": "viewItem == folder"
				}
			]
		}
	}
```
This will show action `extension.deleteFolder` only for items with `contextValue` is `folder`.

___

### description

• `Optional` **description**: string \| boolean

*Defined in [index.d.ts:7994](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7994)*

A human-readable string which is rendered less prominent.
When `true`, it is derived from [resourceUri](#TreeItem.resourceUri) and when `falsy`, it is not shown.

___

### iconPath

• `Optional` **iconPath**: string \| [Uri](_index_d_._plugin_.uri.md) \| { dark: string \| [Uri](_index_d_._plugin_.uri.md) ; light: string \| [Uri](_index_d_._plugin_.uri.md)  } \| [ThemeIcon](_index_d_._plugin_.themeicon.md)

*Defined in [index.d.ts:7988](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7988)*

The icon path or [ThemeIcon](#ThemeIcon) for the tree item.
When `falsy`, [Folder Theme Icon](#ThemeIcon.Folder) is assigned, if item is collapsible otherwise [File Theme Icon](#ThemeIcon.File).
When a file or folder [ThemeIcon](#ThemeIcon) is specified, icon is derived from the current file icon theme for the specified theme icon using [resourceUri](#TreeItem.resourceUri) (if provided).

___

### id

• `Optional` **id**: string

*Defined in [index.d.ts:7981](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7981)*

Optional id for the tree item that has to be unique across tree. The id is used to preserve the selection and expansion state of the tree item.

If not provided, an id is generated using the tree item's label. **Note** that when labels change, ids will change and that selection and expansion state cannot be kept stable anymore.

___

### label

• `Optional` **label**: string

*Defined in [index.d.ts:7974](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7974)*

A human-readable string describing this item. When `falsy`, it is derived from [resourceUri](#TreeItem.resourceUri).

___

### resourceUri

• `Optional` **resourceUri**: [Uri](_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:8002](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8002)*

The [uri](#Uri) of the resource representing this item.

Will be used to derive the [label](#TreeItem.label), when it is not provided.
Will be used to derive the icon from current file icon theme, when [iconPath](#TreeItem.iconPath) has [ThemeIcon](#ThemeIcon) value.

___

### tooltip

• `Optional` **tooltip**: string \| undefined

*Defined in [index.d.ts:8007](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8007)*

The tooltip text when you hover over this item.
