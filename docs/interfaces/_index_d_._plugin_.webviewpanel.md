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

*Defined in [index.d.ts:7411](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7411)*

Whether the panel is active (focused by the user).

___

### iconPath

• `Optional` **iconPath**: [Uri](../classes/_index_d_._plugin_.uri.md) \| { dark: [Uri](../classes/_index_d_._plugin_.uri.md) ; light: [Uri](../classes/_index_d_._plugin_.uri.md)  }

*Defined in [index.d.ts:7390](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7390)*

Icon for the panel shown in UI.

___

### onDidChangeViewState

• `Readonly` **onDidChangeViewState**: [Event](_index_d_._plugin_.event.md)\<[WebviewPanelOnDidChangeViewStateEvent](_index_d_._plugin_.webviewpanelondidchangeviewstateevent.md)>

*Defined in [index.d.ts:7421](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7421)*

Fired when the panel's view state changes.

___

### onDidDispose

• `Readonly` **onDidDispose**: [Event](_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:7431](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7431)*

Fired when the panel is disposed.

This may be because the user closed the panel or because `.dispose()` was
called on it.

Trying to use the panel after it has been disposed throws an exception.

___

### options

• `Readonly` **options**: [WebviewPanelOptions](_index_d_._plugin_.webviewpaneloptions.md)

*Defined in [index.d.ts:7400](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7400)*

Content settings for the webview panel.

___

### title

•  **title**: string

*Defined in [index.d.ts:7385](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7385)*

Title of the panel shown in UI.

___

### viewColumn

• `Optional` `Readonly` **viewColumn**: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md)

*Defined in [index.d.ts:7406](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7406)*

Editor position of the panel. This property is only set if the webview is in
one of the editor view columns.

___

### viewType

• `Readonly` **viewType**: string

*Defined in [index.d.ts:7380](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7380)*

Identifies the type of the webview panel, such as `'markdown.preview'`.

___

### visible

• `Readonly` **visible**: boolean

*Defined in [index.d.ts:7416](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7416)*

Whether the panel is visible.

___

### webview

• `Readonly` **webview**: [Webview](_index_d_._plugin_.webview.md)

*Defined in [index.d.ts:7395](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7395)*

[`Webview`](#Webview) belonging to the panel.

## Methods

### dispose

▸ **dispose**(): any

*Defined in [index.d.ts:7451](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7451)*

Dispose of the webview panel.

This closes the panel if it showing and disposes of the resources owned by the webview.
Webview panels are also disposed when the user closes the webview panel. Both cases
fire the `onDispose` event.

**Returns:** any

___

### reveal

▸ **reveal**(`viewColumn?`: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md), `preserveFocus?`: boolean): void

*Defined in [index.d.ts:7442](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7442)*

Show the webview panel in a given column.

A webview panel may only show in a single column at a time. If it is already showing, this
method moves it to a new column.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`viewColumn?` | [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md) | View column to show the panel in. Shows in the current `viewColumn` if undefined. |
`preserveFocus?` | boolean | When `true`, the webview will not take focus.  |

**Returns:** void
