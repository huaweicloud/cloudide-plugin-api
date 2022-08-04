[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WebviewPanel

# Interface: WebviewPanel

["@codearts/plugin"](../modules/_codearts_plugin_.md).WebviewPanel

## Table of contents

### Properties

- [active](codearts_plugin_.WebviewPanel.md#active)
- [iconPath](codearts_plugin_.WebviewPanel.md#iconpath)
- [onDidChangeViewState](codearts_plugin_.WebviewPanel.md#ondidchangeviewstate)
- [onDidDispose](codearts_plugin_.WebviewPanel.md#ondiddispose)
- [options](codearts_plugin_.WebviewPanel.md#options)
- [showOptions](codearts_plugin_.WebviewPanel.md#showoptions)
- [title](codearts_plugin_.WebviewPanel.md#title)
- [viewColumn](codearts_plugin_.WebviewPanel.md#viewcolumn)
- [viewType](codearts_plugin_.WebviewPanel.md#viewtype)
- [visible](codearts_plugin_.WebviewPanel.md#visible)
- [webview](codearts_plugin_.WebviewPanel.md#webview)

### Methods

- [dispose](codearts_plugin_.WebviewPanel.md#dispose)
- [reveal](codearts_plugin_.WebviewPanel.md#reveal)

## Properties

### active

• `Readonly` **active**: `boolean`

#### Defined in

[index.d.ts:8419](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8419)

___

### iconPath

• `Optional` **iconPath**: [`Uri`](../classes/codearts_plugin_.Uri.md) \| { `dark`: [`Uri`](../classes/codearts_plugin_.Uri.md) ; `light`: [`Uri`](../classes/codearts_plugin_.Uri.md)  }

#### Defined in

[index.d.ts:8392](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8392)

___

### onDidChangeViewState

• `Readonly` **onDidChangeViewState**: [`Event`](codearts_plugin_.Event.md)<[`WebviewPanelOnDidChangeViewStateEvent`](codearts_plugin_.WebviewPanelOnDidChangeViewStateEvent.md)\>

#### Defined in

[index.d.ts:8429](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8429)

___

### onDidDispose

• `Readonly` **onDidDispose**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:8439](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8439)

___

### options

• `Readonly` **options**: [`WebviewPanelOptions`](codearts_plugin_.WebviewPanelOptions.md)

#### Defined in

[index.d.ts:8402](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8402)

___

### showOptions

• `Optional` `Readonly` **showOptions**: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) \| { `area`: `string` ; `preserveFocus?`: `boolean` ; `viewColumn`: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)  }

#### Defined in

[index.d.ts:8408](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8408)

___

### title

• **title**: `string`

#### Defined in

[index.d.ts:8387](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8387)

___

### viewColumn

• `Readonly` **viewColumn**: `undefined` \| [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)

#### Defined in

[index.d.ts:8414](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8414)

___

### viewType

• `Readonly` **viewType**: `string`

#### Defined in

[index.d.ts:8382](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8382)

___

### visible

• `Readonly` **visible**: `boolean`

#### Defined in

[index.d.ts:8424](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8424)

___

### webview

• `Readonly` **webview**: [`Webview`](codearts_plugin_.Webview.md)

#### Defined in

[index.d.ts:8397](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8397)

## Methods

### dispose

▸ **dispose**(): `any`

#### Returns

`any`

#### Defined in

[index.d.ts:8471](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8471)

___

### reveal

▸ **reveal**(`viewColumn?`, `preserveFocus?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewColumn?` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) |  |
| `preserveFocus?` | `boolean` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:8450](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8450)

▸ **reveal**(`area?`, `viewColumn?`, `preserveFocus?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `area?` | `string` |  |
| `viewColumn?` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) |  |
| `preserveFocus?` | `boolean` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:8462](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8462)
