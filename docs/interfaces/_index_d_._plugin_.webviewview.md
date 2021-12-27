**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / WebviewView

# Interface: WebviewView

A webview based view.

## Hierarchy

* **WebviewView**

## Index

### Properties

* [description](_index_d_._plugin_.webviewview.md#description)
* [onDidChangeVisibility](_index_d_._plugin_.webviewview.md#ondidchangevisibility)
* [onDidDispose](_index_d_._plugin_.webviewview.md#ondiddispose)
* [title](_index_d_._plugin_.webviewview.md#title)
* [viewType](_index_d_._plugin_.webviewview.md#viewtype)
* [visible](_index_d_._plugin_.webviewview.md#visible)
* [webview](_index_d_._plugin_.webviewview.md#webview)

### Methods

* [show](_index_d_._plugin_.webviewview.md#show)

## Properties

### description

• `Optional` **description**: string

*Defined in [index.d.ts:7539](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7539)*

Human-readable string which is rendered less prominently in the title.

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [Event](_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:7568](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7568)*

Event fired when the visibility of the view changes.

Actions that trigger a visibility change:

- The view is collapsed or expanded.
- The user switches to a different view group in the sidebar or panel.

Note that hiding a view using the context menu instead disposes of the view and fires `onDidDispose`.

___

### onDidDispose

• `Readonly` **onDidDispose**: [Event](_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:7549](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7549)*

Event fired when the view is disposed.

Views are disposed when they are explicitly hidden by a user (this happens when a user
right clicks in a view and unchecks the webview view).

Trying to use the view after it has been disposed throws an exception.

___

### title

• `Optional` **title**: string

*Defined in [index.d.ts:7534](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7534)*

View title displayed in the UI.

The view title is initially taken from the extension `package.json` contribution.

___

### viewType

• `Readonly` **viewType**: string

*Defined in [index.d.ts:7522](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7522)*

Identifies the type of the webview view, such as `'hexEditor.dataView'`.

___

### visible

• `Readonly` **visible**: boolean

*Defined in [index.d.ts:7556](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7556)*

Tracks if the webview is currently visible.

Views are visible when they are on the screen and expanded.

___

### webview

• `Readonly` **webview**: [Webview](_index_d_._plugin_.webview.md)

*Defined in [index.d.ts:7527](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7527)*

The underlying webview for the view.

## Methods

### show

▸ **show**(`preserveFocus?`: boolean): void

*Defined in [index.d.ts:7577](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7577)*

Reveal the view in the UI.

If the view is collapsed, this will expand it.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`preserveFocus?` | boolean | When `true` the view will not take focus.  |

**Returns:** void
