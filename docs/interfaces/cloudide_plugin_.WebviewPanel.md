[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / WebviewPanel

# Interface: WebviewPanel

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).WebviewPanel

A panel that contains a webview.

## Table of contents

### Properties

- [active](cloudide_plugin_.WebviewPanel.md#active)
- [iconPath](cloudide_plugin_.WebviewPanel.md#iconpath)
- [onDidChangeViewState](cloudide_plugin_.WebviewPanel.md#ondidchangeviewstate)
- [onDidDispose](cloudide_plugin_.WebviewPanel.md#ondiddispose)
- [options](cloudide_plugin_.WebviewPanel.md#options)
- [showOptions](cloudide_plugin_.WebviewPanel.md#showoptions)
- [title](cloudide_plugin_.WebviewPanel.md#title)
- [viewColumn](cloudide_plugin_.WebviewPanel.md#viewcolumn)
- [viewType](cloudide_plugin_.WebviewPanel.md#viewtype)
- [visible](cloudide_plugin_.WebviewPanel.md#visible)
- [webview](cloudide_plugin_.WebviewPanel.md#webview)

### Methods

- [dispose](cloudide_plugin_.WebviewPanel.md#dispose)
- [reveal](cloudide_plugin_.WebviewPanel.md#reveal)

## Properties

### active

• `Readonly` **active**: `boolean`

Whether the panel is active (focused by the user).

#### Defined in

[index.d.ts:3571](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3571)

___

### iconPath

• `Optional` **iconPath**: [`Uri`](../classes/cloudide_plugin_.Uri.md) \| { `dark`: [`Uri`](../classes/cloudide_plugin_.Uri.md) ; `light`: [`Uri`](../classes/cloudide_plugin_.Uri.md)  }

Icon for the panel shown in UI.

#### Defined in

[index.d.ts:3546](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3546)

___

### onDidChangeViewState

• `Readonly` **onDidChangeViewState**: [`Event`](cloudide_plugin_.Event.md)<[`WebviewPanelOnDidChangeViewStateEvent`](cloudide_plugin_.WebviewPanelOnDidChangeViewStateEvent.md)\>

Fired when the panel's view state changes.

#### Defined in

[index.d.ts:3581](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3581)

___

### onDidDispose

• `Readonly` **onDidDispose**: [`Event`](cloudide_plugin_.Event.md)<`void`\>

Fired when the panel is disposed.

This may be because the user closed the panel or because `.dispose()` was
called on it.

Trying to use the panel after it has been disposed throws an exception.

#### Defined in

[index.d.ts:3591](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3591)

___

### options

• `Readonly` **options**: [`WebviewPanelOptions`](cloudide_plugin_.WebviewPanelOptions.md)

Content settings for the webview panel.

#### Defined in

[index.d.ts:3556](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3556)

___

### showOptions

• `Optional` `Readonly` **showOptions**: [`WebviewPanelShowOptions`](cloudide_plugin_.WebviewPanelShowOptions.md)

Settings to determine where webview panel will be reside

#### Defined in

[index.d.ts:3561](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3561)

___

### title

• **title**: `string`

Title of the panel shown in UI.

#### Defined in

[index.d.ts:3541](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3541)

___

### viewColumn

• `Optional` `Readonly` **viewColumn**: [`ViewColumn`](../enums/cloudide_plugin_.ViewColumn.md)

Editor position of the panel. This property is only set if the webview is in
one of the editor view columns.

#### Defined in

[index.d.ts:3566](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3566)

___

### viewType

• `Readonly` **viewType**: `string`

Identifies the type of the webview panel, such as `'markdown.preview'`.

#### Defined in

[index.d.ts:3536](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3536)

___

### visible

• `Readonly` **visible**: `boolean`

Whether the panel is visible.

#### Defined in

[index.d.ts:3576](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3576)

___

### webview

• `Readonly` **webview**: [`Webview`](cloudide_plugin_.Webview.md)

Webview belonging to the panel.

#### Defined in

[index.d.ts:3551](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3551)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose of the webview panel.

This closes the panel if it showing and disposes of the resources owned by the webview.
Webview panels are also disposed when the user closes the webview panel. Both cases
fire the `onDispose` event.

#### Returns

`void`

#### Defined in

[index.d.ts:3623](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3623)

___

### reveal

▸ **reveal**(`viewColumn?`, `preserveFocus?`): `void`

Show the webview panel in a given column.

A webview panel may only show in a single column at a time. If it is already showing, this
method moves it to a new column.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewColumn?` | [`ViewColumn`](../enums/cloudide_plugin_.ViewColumn.md) | View column to show the panel in. Shows in the current `viewColumn` if undefined. |
| `preserveFocus?` | `boolean` | When `true`, the webview will not take focus. |

#### Returns

`void`

#### Defined in

[index.d.ts:3602](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3602)

▸ **reveal**(`area?`, `viewColumn?`, `preserveFocus?`): `void`

Show the webview panel according to a given options.

A webview panel may only show in a single column at a time. If it is already showing, this
method moves it to a new column.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `area?` | [`WebviewPanelTargetArea`](../enums/cloudide_plugin_.WebviewPanelTargetArea.md) | target area where webview panel will be resided. Shows in the 'WebviewPanelTargetArea.Main' area if undefined. |
| `viewColumn?` | [`ViewColumn`](../enums/cloudide_plugin_.ViewColumn.md) | View column to show the panel in. Shows in the current `viewColumn` if undefined. |
| `preserveFocus?` | `boolean` | When `true`, the webview will not take focus. |

#### Returns

`void`

#### Defined in

[index.d.ts:3614](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3614)
