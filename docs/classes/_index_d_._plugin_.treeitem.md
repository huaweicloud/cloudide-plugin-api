**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TreeItem

# Class: TreeItem

## Hierarchy

* **TreeItem**

## Index

### Constructors

* [constructor](_index_d_._plugin_.treeitem.md#constructor)

### Properties

* [accessibilityInformation](_index_d_._plugin_.treeitem.md#accessibilityinformation)
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

\+ **new TreeItem**(`label`: string \| [TreeItemLabel](../interfaces/_index_d_._plugin_.treeitemlabel.md), `collapsibleState?`: [TreeItemCollapsibleState](../enums/_index_d_._plugin_.treeitemcollapsiblestate.md)): [TreeItem](_index_d_._plugin_.treeitem.md)

*Defined in [index.d.ts:9302](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9302)*

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`label` | string \| [TreeItemLabel](../interfaces/_index_d_._plugin_.treeitemlabel.md) | A human-readable string describing this item |
`collapsibleState?` | [TreeItemCollapsibleState](../enums/_index_d_._plugin_.treeitemcollapsiblestate.md) | (#TreeItemCollapsibleState) of the tree item. Default is [TreeItemCollapsibleState.None](#TreeItemCollapsibleState.None)  |

**Returns:** [TreeItem](_index_d_._plugin_.treeitem.md)

\+ **new TreeItem**(`resourceUri`: [Uri](_index_d_._plugin_.uri.md), `collapsibleState?`: [TreeItemCollapsibleState](../enums/_index_d_._plugin_.treeitemcollapsiblestate.md)): [TreeItem](_index_d_._plugin_.treeitem.md)

*Defined in [index.d.ts:9308](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9308)*

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`resourceUri` | [Uri](_index_d_._plugin_.uri.md) | The [uri](#Uri) of the resource representing this item. |
`collapsibleState?` | [TreeItemCollapsibleState](../enums/_index_d_._plugin_.treeitemcollapsiblestate.md) | (#TreeItemCollapsibleState) of the tree item. Default is [TreeItemCollapsibleState.None](#TreeItemCollapsibleState.None)  |

**Returns:** [TreeItem](_index_d_._plugin_.treeitem.md)

## Properties

### accessibilityInformation

• `Optional` **accessibilityInformation**: [AccessibilityInformation](../interfaces/_index_d_._plugin_.accessibilityinformation.md)

*Defined in [index.d.ts:9302](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9302)*

Accessibility information used when screen reader interacts with this tree item.
Generally, a TreeItem has no need to set the `role` of the accessibilityInformation;
however, there are cases where a TreeItem is not displayed in a tree-like way where setting the `role` may make sense.

___

### collapsibleState

• `Optional` **collapsibleState**: [TreeItemCollapsibleState](../enums/_index_d_._plugin_.treeitemcollapsiblestate.md)

*Defined in [index.d.ts:9275](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9275)*

[TreeItemCollapsibleState](#TreeItemCollapsibleState) of the tree item.

___

### command

• `Optional` **command**: [Command](../interfaces/_index_d_._plugin_.command.md)

*Defined in [index.d.ts:9270](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9270)*

The [command](#Command) that should be executed when the tree item is selected.

Please use `vscode.open` or `vscode.diff` as command IDs when the tree item is opening
something in the editor. Using these commands ensures that the resulting editor will
appear consistent with how other built-in trees open editors.

___

### contextValue

• `Optional` **contextValue**: string

*Defined in [index.d.ts:9295](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9295)*

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

*Defined in [index.d.ts:9248](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9248)*

A human-readable string which is rendered less prominent.
When `true`, it is derived from [resourceUri](#TreeItem.resourceUri) and when `falsy`, it is not shown.

___

### iconPath

• `Optional` **iconPath**: string \| [Uri](_index_d_._plugin_.uri.md) \| { dark: string \| [Uri](_index_d_._plugin_.uri.md) ; light: string \| [Uri](_index_d_._plugin_.uri.md)  } \| [ThemeIcon](_index_d_._plugin_.themeicon.md)

*Defined in [index.d.ts:9242](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9242)*

The icon path or [ThemeIcon](#ThemeIcon) for the tree item.
When `falsy`, [Folder Theme Icon](#ThemeIcon.Folder) is assigned, if item is collapsible otherwise [File Theme Icon](#ThemeIcon.File).
When a file or folder [ThemeIcon](#ThemeIcon) is specified, icon is derived from the current file icon theme for the specified theme icon using [resourceUri](#TreeItem.resourceUri) (if provided).

___

### id

• `Optional` **id**: string

*Defined in [index.d.ts:9235](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9235)*

Optional id for the tree item that has to be unique across tree. The id is used to preserve the selection and expansion state of the tree item.

If not provided, an id is generated using the tree item's label. **Note** that when labels change, ids will change and that selection and expansion state cannot be kept stable anymore.

___

### label

• `Optional` **label**: string \| [TreeItemLabel](../interfaces/_index_d_._plugin_.treeitemlabel.md)

*Defined in [index.d.ts:9228](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9228)*

A human-readable string describing this item. When `falsy`, it is derived from [resourceUri](#TreeItem.resourceUri).

___

### resourceUri

• `Optional` **resourceUri**: [Uri](_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:9256](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9256)*

The [uri](#Uri) of the resource representing this item.

Will be used to derive the [label](#TreeItem.label), when it is not provided.
Will be used to derive the icon from current file icon theme, when [iconPath](#TreeItem.iconPath) has [ThemeIcon](#ThemeIcon) value.

___

### tooltip

• `Optional` **tooltip**: string \| [MarkdownString](_index_d_._plugin_.markdownstring.md) \| undefined

*Defined in [index.d.ts:9261](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9261)*

The tooltip text when you hover over this item.
