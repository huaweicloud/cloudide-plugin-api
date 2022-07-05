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

[index.d.ts:10387](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10387)

• **new TreeItem**(`resourceUri`, `collapsibleState?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `resourceUri` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `collapsibleState?` | [`TreeItemCollapsibleState`](../enums/codearts_plugin_.TreeItemCollapsibleState.md) |  |

#### Defined in

[index.d.ts:10393](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10393)

## Properties

### accessibilityInformation

• `Optional` **accessibilityInformation**: [`AccessibilityInformation`](../interfaces/codearts_plugin_.AccessibilityInformation.md)

#### Defined in

[index.d.ts:10381](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10381)

___

### collapsibleState

• `Optional` **collapsibleState**: [`TreeItemCollapsibleState`](../enums/codearts_plugin_.TreeItemCollapsibleState.md)

#### Defined in

[index.d.ts:10354](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10354)

___

### command

• `Optional` **command**: [`Command`](../interfaces/codearts_plugin_.Command.md)

#### Defined in

[index.d.ts:10349](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10349)

___

### contextValue

• `Optional` **contextValue**: `string`

#### Defined in

[index.d.ts:10374](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10374)

___

### description

• `Optional` **description**: `string` \| `boolean`

#### Defined in

[index.d.ts:10327](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10327)

___

### iconPath

• `Optional` **iconPath**: `string` \| [`Uri`](codearts_plugin_.Uri.md) \| [`ThemeIcon`](codearts_plugin_.ThemeIcon.md) \| { `dark`: `string` \| [`Uri`](codearts_plugin_.Uri.md) ; `light`: `string` \| [`Uri`](codearts_plugin_.Uri.md)  }

#### Defined in

[index.d.ts:10321](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10321)

___

### id

• `Optional` **id**: `string`

#### Defined in

[index.d.ts:10314](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10314)

___

### label

• `Optional` **label**: `string` \| [`TreeItemLabel`](../interfaces/codearts_plugin_.TreeItemLabel.md)

#### Defined in

[index.d.ts:10307](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10307)

___

### resourceUri

• `Optional` **resourceUri**: [`Uri`](codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:10335](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10335)

___

### tooltip

• `Optional` **tooltip**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:10340](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L10340)
