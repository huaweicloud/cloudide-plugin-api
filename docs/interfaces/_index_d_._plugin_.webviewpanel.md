**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / WebviewPanel

# Interface: WebviewPanel

A panel that contains a webview.

## Hierarchy

* **WebviewPanel**

## Index

### Properties

* [active](_index_d_._plugin_.webviewpanel.md#active)
* [iconPath](_index_d_._plugin_.webviewpanel.md#iconpath)
* [onDidChangeViewState](_index_d_._plugin_.webviewpanel.md#ondidchangeviewstate)
* [onDidDispose](_index_d_._plugin_.webviewpanel.md#ondiddispose)
* [options](_index_d_._plugin_.webviewpanel.md#options)
* [title](_index_d_._plugin_.webviewpanel.md#title)
* [viewColumn](_index_d_._plugin_.webviewpanel.md#viewcolumn)
* [viewType](_index_d_._plugin_.webviewpanel.md#viewtype)
* [visible](_index_d_._plugin_.webviewpanel.md#visible)
* [webview](_index_d_._plugin_.webviewpanel.md#webview)

### Methods

* [dispose](_index_d_._plugin_.webviewpanel.md#dispose)
* [reveal](_index_d_._plugin_.webviewpanel.md#reveal)

## Properties

### active

• `Readonly` **active**: boolean

*Defined in [index.d.ts:7414](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7414)*

Whether the panel is active (focused by the user).

___

### iconPath

• `Optional` **iconPath**: [Uri](../classes/_index_d_._plugin_.uri.md) \| { dark: [Uri](../classes/_index_d_._plugin_.uri.md) ; light: [Uri](../classes/_index_d_._plugin_.uri.md)  }

*Defined in [index.d.ts:7393](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7393)*

Icon for the panel shown in UI.

___

### onDidChangeViewState

• `Readonly` **onDidChangeViewState**: [Event](_index_d_._plugin_.event.md)\<[WebviewPanelOnDidChangeViewStateEvent](_index_d_._plugin_.webviewpanelondidchangeviewstateevent.md)>

*Defined in [index.d.ts:7424](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7424)*

Fired when the panel's view state changes.

___

### onDidDispose

• `Readonly` **onDidDispose**: [Event](_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:7434](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7434)*

Fired when the panel is disposed.

This may be because the user closed the panel or because `.dispose()` was
called on it.

Trying to use the panel after it has been disposed throws an exception.

___

### options

• `Readonly` **options**: [WebviewPanelOptions](_index_d_._plugin_.webviewpaneloptions.md)

*Defined in [index.d.ts:7403](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7403)*

Content settings for the webview panel.

___

### title

•  **title**: string

*Defined in [index.d.ts:7388](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7388)*

Title of the panel shown in UI.

___

### viewColumn

• `Optional` `Readonly` **viewColumn**: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md)

*Defined in [index.d.ts:7409](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7409)*

Editor position of the panel. This property is only set if the webview is in
one of the editor view columns.

___

### viewType

• `Readonly` **viewType**: string

*Defined in [index.d.ts:7383](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7383)*

Identifies the type of the webview panel, such as `'markdown.preview'`.

___

### visible

• `Readonly` **visible**: boolean

*Defined in [index.d.ts:7419](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7419)*

Whether the panel is visible.

___

### webview

• `Readonly` **webview**: [Webview](_index_d_._plugin_.webview.md)

*Defined in [index.d.ts:7398](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7398)*

[`Webview`](#Webview) belonging to the panel.

## Methods

### dispose

▸ **dispose**(): any

*Defined in [index.d.ts:7454](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7454)*

Dispose of the webview panel.

This closes the panel if it showing and disposes of the resources owned by the webview.
Webview panels are also disposed when the user closes the webview panel. Both cases
fire the `onDispose` event.

**Returns:** any

___

### reveal

▸ **reveal**(`viewColumn?`: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md), `preserveFocus?`: boolean): void

*Defined in [index.d.ts:7445](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7445)*

Show the webview panel in a given column.

A webview panel may only show in a single column at a time. If it is already showing, this
method moves it to a new column.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`viewColumn?` | [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md) | View column to show the panel in. Shows in the current `viewColumn` if undefined. |
`preserveFocus?` | boolean | When `true`, the webview will not take focus.  |

**Returns:** void
