[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TreeItem

# Class: TreeItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).TreeItem

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TreeItem.md#constructor)

### Properties

- [accessibilityInformation](codearts_plugin_.TreeItem.md#accessibilityinformation)
- [collapsibleState](codearts_plugin_.TreeItem.md#collapsiblestate)
- [command](codearts_plugin_.TreeItem.md#command)
- [contextValue](codearts_plugin_.TreeItem.md#contextvalue)
- [description](codearts_plugin_.TreeItem.md#description)
- [iconPath](codearts_plugin_.TreeItem.md#iconpath)
- [id](codearts_plugin_.TreeItem.md#id)
- [label](codearts_plugin_.TreeItem.md#label)
- [resourceUri](codearts_plugin_.TreeItem.md#resourceuri)
- [tooltip](codearts_plugin_.TreeItem.md#tooltip)

## Constructors

### constructor

• **new TreeItem**(`label`, `collapsibleState?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` \| [`TreeItemLabel`](../interfaces/codearts_plugin_.TreeItemLabel.md) | A human-readable string describing this item |
| `collapsibleState?` | [`TreeItemCollapsibleState`](../enums/codearts_plugin_.TreeItemCollapsibleState.md) | [TreeItemCollapsibleState](../enums/codearts_plugin_.TreeItemCollapsibleState.md) of the tree item. Default is [None](../enums/codearts_plugin_.TreeItemCollapsibleState.md#none) |

#### Defined in

[index.d.ts:10803](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10803)

• **new TreeItem**(`resourceUri`, `collapsibleState?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `resourceUri` | [`Uri`](codearts_plugin_.Uri.md) | The [Uri](codearts_plugin_.Uri.md) of the resource representing this item. |
| `collapsibleState?` | [`TreeItemCollapsibleState`](../enums/codearts_plugin_.TreeItemCollapsibleState.md) | [TreeItemCollapsibleState](../enums/codearts_plugin_.TreeItemCollapsibleState.md) of the tree item. Default is [None](../enums/codearts_plugin_.TreeItemCollapsibleState.md#none) |

#### Defined in

[index.d.ts:10809](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10809)

## Properties

### accessibilityInformation

• `Optional` **accessibilityInformation**: [`AccessibilityInformation`](../interfaces/codearts_plugin_.AccessibilityInformation.md)

Accessibility information used when screen reader interacts with this tree item.
Generally, a TreeItem has no need to set the `role` of the accessibilityInformation;
however, there are cases where a TreeItem is not displayed in a tree-like way where setting the `role` may make sense.

#### Defined in

[index.d.ts:10797](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10797)

___

### collapsibleState

• `Optional` **collapsibleState**: [`TreeItemCollapsibleState`](../enums/codearts_plugin_.TreeItemCollapsibleState.md)

[TreeItemCollapsibleState](../enums/codearts_plugin_.TreeItemCollapsibleState.md) of the tree item.

#### Defined in

[index.d.ts:10770](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10770)

___

### command

• `Optional` **command**: [`Command`](../interfaces/codearts_plugin_.Command.md)

The [Command](../interfaces/codearts_plugin_.Command.md) that should be executed when the tree item is selected.

Please use `vscode.open` or `vscode.diff` as command IDs when the tree item is opening
something in the editor. Using these commands ensures that the resulting editor will
appear consistent with how other built-in trees open editors.

#### Defined in

[index.d.ts:10765](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10765)

___

### contextValue

• `Optional` **contextValue**: `string`

Context value of the tree item. This can be used to contribute item specific actions in the tree.
For example, a tree item is given a context value as `folder`. When contributing actions to `view/item/context`
using `menus` extension point, you can specify context value for key `viewItem` in `when` expression like `viewItem == folder`.
```json
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

[index.d.ts:10790](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10790)

___

### description

• `Optional` **description**: `string` \| `boolean`

A human-readable string which is rendered less prominent.
When `true`, it is derived from [resourceUri](codearts_plugin_.TreeItem.md#resourceuri) and when `falsy`, it is not shown.

#### Defined in

[index.d.ts:10743](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10743)

___

### iconPath

• `Optional` **iconPath**: `string` \| [`Uri`](codearts_plugin_.Uri.md) \| [`ThemeIcon`](codearts_plugin_.ThemeIcon.md) \| { `dark`: `string` \| [`Uri`](codearts_plugin_.Uri.md) ; `light`: `string` \| [`Uri`](codearts_plugin_.Uri.md)  }

The icon path or [ThemeIcon](codearts_plugin_.ThemeIcon.md) for the tree item.
When `falsy`, [Folder Theme Icon](codearts_plugin_.ThemeIcon.md#folder) is assigned, if item is collapsible otherwise [File Theme Icon](codearts_plugin_.ThemeIcon.md#file).
When a file or folder [ThemeIcon](codearts_plugin_.ThemeIcon.md) is specified, icon is derived from the current file icon theme for the specified theme icon using [resourceUri](codearts_plugin_.TreeItem.md#resourceuri) (if provided).

#### Defined in

[index.d.ts:10737](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10737)

___

### id

• `Optional` **id**: `string`

Optional id for the tree item that has to be unique across tree. The id is used to preserve the selection and expansion state of the tree item.

If not provided, an id is generated using the tree item's label. **Note** that when labels change, ids will change and that selection and expansion state cannot be kept stable anymore.

#### Defined in

[index.d.ts:10730](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10730)

___

### label

• `Optional` **label**: `string` \| [`TreeItemLabel`](../interfaces/codearts_plugin_.TreeItemLabel.md)

A human-readable string describing this item. When `falsy`, it is derived from [resourceUri](codearts_plugin_.TreeItem.md#resourceuri).

#### Defined in

[index.d.ts:10723](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10723)

___

### resourceUri

• `Optional` **resourceUri**: [`Uri`](codearts_plugin_.Uri.md)

The [Uri](codearts_plugin_.Uri.md) of the resource representing this item.

Will be used to derive the [label](codearts_plugin_.TreeItem.md#label), when it is not provided.
Will be used to derive the icon from current file icon theme, when [iconPath](codearts_plugin_.TreeItem.md#iconpath) has [ThemeIcon](codearts_plugin_.ThemeIcon.md) value.

#### Defined in

[index.d.ts:10751](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10751)

___

### tooltip

• `Optional` **tooltip**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

The tooltip text when you hover over this item.

#### Defined in

[index.d.ts:10756](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10756)
