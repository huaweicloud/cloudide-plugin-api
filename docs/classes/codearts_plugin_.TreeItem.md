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
| `label` | `string` \| [`TreeItemLabel`](../interfaces/codearts_plugin_.TreeItemLabel.md) |  |
| `collapsibleState?` | [`TreeItemCollapsibleState`](../enums/codearts_plugin_.TreeItemCollapsibleState.md) |  |

#### Defined in

[index.d.ts:10417](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10417)

• **new TreeItem**(`resourceUri`, `collapsibleState?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `resourceUri` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `collapsibleState?` | [`TreeItemCollapsibleState`](../enums/codearts_plugin_.TreeItemCollapsibleState.md) |  |

#### Defined in

[index.d.ts:10423](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10423)

## Properties

### accessibilityInformation

• `Optional` **accessibilityInformation**: [`AccessibilityInformation`](../interfaces/codearts_plugin_.AccessibilityInformation.md)

#### Defined in

[index.d.ts:10411](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10411)

___

### collapsibleState

• `Optional` **collapsibleState**: [`TreeItemCollapsibleState`](../enums/codearts_plugin_.TreeItemCollapsibleState.md)

#### Defined in

[index.d.ts:10384](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10384)

___

### command

• `Optional` **command**: [`Command`](../interfaces/codearts_plugin_.Command.md)

#### Defined in

[index.d.ts:10379](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10379)

___

### contextValue

• `Optional` **contextValue**: `string`

#### Defined in

[index.d.ts:10404](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10404)

___

### description

• `Optional` **description**: `string` \| `boolean`

#### Defined in

[index.d.ts:10357](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10357)

___

### iconPath

• `Optional` **iconPath**: `string` \| [`Uri`](codearts_plugin_.Uri.md) \| [`ThemeIcon`](codearts_plugin_.ThemeIcon.md) \| { `dark`: `string` \| [`Uri`](codearts_plugin_.Uri.md) ; `light`: `string` \| [`Uri`](codearts_plugin_.Uri.md)  }

#### Defined in

[index.d.ts:10351](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10351)

___

### id

• `Optional` **id**: `string`

#### Defined in

[index.d.ts:10344](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10344)

___

### label

• `Optional` **label**: `string` \| [`TreeItemLabel`](../interfaces/codearts_plugin_.TreeItemLabel.md)

#### Defined in

[index.d.ts:10337](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10337)

___

### resourceUri

• `Optional` **resourceUri**: [`Uri`](codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:10365](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10365)

___

### tooltip

• `Optional` **tooltip**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:10370](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10370)
