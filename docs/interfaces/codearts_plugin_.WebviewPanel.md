[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WebviewPanel

# Interface: WebviewPanel

["@codearts/plugin"](../modules/_codearts_plugin_.md).WebviewPanel

A panel that contains a webview.

## Table of contents

### Properties

- [active](codearts_plugin_.WebviewPanel.md#active)
- [iconPath](codearts_plugin_.WebviewPanel.md#iconpath)
- [onDidChangeViewState](codearts_plugin_.WebviewPanel.md#ondidchangeviewstate)
- [onDidDispose](codearts_plugin_.WebviewPanel.md#ondiddispose)
- [options](codearts_plugin_.WebviewPanel.md#options)
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

Whether the panel is active (focused by the user).

#### Defined in

[index.d.ts:8468](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8468)

___

### iconPath

• `Optional` **iconPath**: [`Uri`](../classes/codearts_plugin_.Uri.md) \| { `dark`: [`Uri`](../classes/codearts_plugin_.Uri.md) ; `light`: [`Uri`](../classes/codearts_plugin_.Uri.md)  }

Icon for the panel shown in UI.

#### Defined in

[index.d.ts:8447](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8447)

___

### onDidChangeViewState

• `Readonly` **onDidChangeViewState**: [`Event`](codearts_plugin_.Event.md)<[`WebviewPanelOnDidChangeViewStateEvent`](codearts_plugin_.WebviewPanelOnDidChangeViewStateEvent.md)\>

Fired when the panel's view state changes.

#### Defined in

[index.d.ts:8478](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8478)

___

### onDidDispose

• `Readonly` **onDidDispose**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the panel is disposed.

This may be because the user closed the panel or because `.dispose()` was
called on it.

Trying to use the panel after it has been disposed throws an exception.

#### Defined in

[index.d.ts:8488](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8488)

___

### options

• `Readonly` **options**: [`WebviewPanelOptions`](codearts_plugin_.WebviewPanelOptions.md)

Content settings for the webview panel.

#### Defined in

[index.d.ts:8457](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8457)

___

### title

• **title**: `string`

Title of the panel shown in UI.

#### Defined in

[index.d.ts:8442](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8442)

___

### viewColumn

• `Readonly` **viewColumn**: `undefined` \| [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)

Editor position of the panel. This property is only set if the webview is in
one of the editor view columns.

#### Defined in

[index.d.ts:8463](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8463)

___

### viewType

• `Readonly` **viewType**: `string`

Identifies the type of the webview panel, such as `'markdown.preview'`.

#### Defined in

[index.d.ts:8437](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8437)

___

### visible

• `Readonly` **visible**: `boolean`

Whether the panel is visible.

#### Defined in

[index.d.ts:8473](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8473)

___

### webview

• `Readonly` **webview**: [`Webview`](codearts_plugin_.Webview.md)

[`Webview`](codearts_plugin_.Webview.md) belonging to the panel.

#### Defined in

[index.d.ts:8452](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8452)

## Methods

### dispose

▸ **dispose**(): `any`

Dispose of the webview panel.

This closes the panel if it showing and disposes of the resources owned by the webview.
Webview panels are also disposed when the user closes the webview panel. Both cases
fire the `onDispose` event.

#### Returns

`any`

#### Defined in

[index.d.ts:8508](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8508)

___

### reveal

▸ **reveal**(`viewColumn?`, `preserveFocus?`): `void`

Show the webview panel in a given column.

A webview panel may only show in a single column at a time. If it is already showing, this
method moves it to a new column.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewColumn?` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) | View column to show the panel in. Shows in the current `viewColumn` if undefined. |
| `preserveFocus?` | `boolean` | When `true`, the webview will not take focus. |

#### Returns

`void`

#### Defined in

[index.d.ts:8499](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8499)
