[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TreeItem

# Class: TreeItem

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TreeItem

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.TreeItem.md#constructor)

### Properties

- [collapsibleState](cloudide_plugin_.TreeItem.md#collapsiblestate)
- [command](cloudide_plugin_.TreeItem.md#command)
- [contextValue](cloudide_plugin_.TreeItem.md#contextvalue)
- [description](cloudide_plugin_.TreeItem.md#description)
- [iconPath](cloudide_plugin_.TreeItem.md#iconpath)
- [id](cloudide_plugin_.TreeItem.md#id)
- [label](cloudide_plugin_.TreeItem.md#label)
- [resourceUri](cloudide_plugin_.TreeItem.md#resourceuri)
- [tooltip](cloudide_plugin_.TreeItem.md#tooltip)

## Constructors

### constructor

• **new TreeItem**(`label`, `collapsibleState?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` | A human-readable string describing this item |
| `collapsibleState?` | [`TreeItemCollapsibleState`](../enums/cloudide_plugin_.TreeItemCollapsibleState.md) | [TreeItemCollapsibleState](#TreeItemCollapsibleState) of the tree item. Default is [TreeItemCollapsibleState.None](#TreeItemCollapsibleState.None) |

#### Defined in

[index.d.ts:5378](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5378)

• **new TreeItem**(`resourceUri`, `collapsibleState?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `resourceUri` | [`Uri`](cloudide_plugin_.Uri.md) | The [uri](#Uri) of the resource representing this item. |
| `collapsibleState?` | [`TreeItemCollapsibleState`](../enums/cloudide_plugin_.TreeItemCollapsibleState.md) | [TreeItemCollapsibleState](#TreeItemCollapsibleState) of the tree item. Default is [TreeItemCollapsibleState.None](#TreeItemCollapsibleState.None) |

#### Defined in

[index.d.ts:5384](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5384)

## Properties

### collapsibleState

• `Optional` **collapsibleState**: [`TreeItemCollapsibleState`](../enums/cloudide_plugin_.TreeItemCollapsibleState.md)

[TreeItemCollapsibleState](#TreeItemCollapsibleState) of the tree item.

#### Defined in

[index.d.ts:5352](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5352)

___

### command

• `Optional` **command**: [`Command`](../interfaces/cloudide_plugin_.Command.md)

The [command](#Command) which should be run when the tree item is selected.

#### Defined in

[index.d.ts:5347](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5347)

___

### contextValue

• `Optional` **contextValue**: `string`

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

#### Defined in

[index.d.ts:5372](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5372)

___

### description

• `Optional` **description**: `string` \| `boolean`

A human readable string which is rendered less prominent.
When `true`, it is derived from [resourceUri](#TreeItem.resourceUri) and when `falsy`, it is not shown.

#### Defined in

[index.d.ts:5329](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5329)

___

### iconPath

• `Optional` **iconPath**: `string` \| [`Uri`](cloudide_plugin_.Uri.md) \| [`ThemeIcon`](cloudide_plugin_.ThemeIcon.md) \| { `dark`: `string` \| [`Uri`](cloudide_plugin_.Uri.md) ; `light`: `string` \| [`Uri`](cloudide_plugin_.Uri.md)  }

The icon path or [ThemeIcon](#ThemeIcon) for the tree item.
When `falsy`, [Folder Theme Icon](#ThemeIcon.Folder) is assigned, if item is collapsible otherwise [File Theme Icon](#ThemeIcon.File).
When a [ThemeIcon](#ThemeIcon) is specified, icon is derived from the current file icon theme for the specified theme icon using [resourceUri](#TreeItem.resourceUri) (if provided).

#### Defined in

[index.d.ts:5323](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5323)

___

### id

• `Optional` **id**: `string`

Optional id for the tree item that has to be unique across tree. The id is used to preserve the selection and expansion state of the tree item.

If not provided, an id is generated using the tree item's label. **Note** that when labels change, ids will change and that selection and expansion state cannot be kept stable anymore.

#### Defined in

[index.d.ts:5316](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5316)

___

### label

• `Optional` **label**: `string`

A human-readable string describing this item. When `falsy`, it is derived from [resourceUri](#TreeItem.resourceUri).

#### Defined in

[index.d.ts:5309](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5309)

___

### resourceUri

• `Optional` **resourceUri**: [`Uri`](cloudide_plugin_.Uri.md)

The [uri](#Uri) of the resource representing this item.

Will be used to derive the [label](#TreeItem.label), when it is not provided.
Will be used to derive the icon from current icon theme, when [iconPath](#TreeItem.iconPath) has [ThemeIcon](#ThemeIcon) value.

#### Defined in

[index.d.ts:5337](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5337)

___

### tooltip

• `Optional` **tooltip**: `string`

The tooltip text when you hover over this item.

#### Defined in

[index.d.ts:5342](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5342)
