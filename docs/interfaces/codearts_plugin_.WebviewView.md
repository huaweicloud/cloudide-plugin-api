[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WebviewView

# Interface: WebviewView

["@codearts/plugin"](../modules/_codearts_plugin_.md).WebviewView

A webview based view.

## Table of contents

### Properties

- [description](codearts_plugin_.WebviewView.md#description)
- [onDidChangeVisibility](codearts_plugin_.WebviewView.md#ondidchangevisibility)
- [onDidDispose](codearts_plugin_.WebviewView.md#ondiddispose)
- [title](codearts_plugin_.WebviewView.md#title)
- [viewType](codearts_plugin_.WebviewView.md#viewtype)
- [visible](codearts_plugin_.WebviewView.md#visible)
- [webview](codearts_plugin_.WebviewView.md#webview)

### Methods

- [show](codearts_plugin_.WebviewView.md#show)

## Properties

### description

• `Optional` **description**: `string`

Human-readable string which is rendered less prominently in the title.

#### Defined in

[index.d.ts:8654](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8654)

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Event fired when the visibility of the view changes.

Actions that trigger a visibility change:

- The view is collapsed or expanded.
- The user switches to a different view group in the sidebar or panel.

Note that hiding a view using the context menu instead disposes of the view and fires `onDidDispose`.

#### Defined in

[index.d.ts:8683](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8683)

___

### onDidDispose

• `Readonly` **onDidDispose**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Event fired when the view is disposed.

Views are disposed when they are explicitly hidden by a user (this happens when a user
right clicks in a view and unchecks the webview view).

Trying to use the view after it has been disposed throws an exception.

#### Defined in

[index.d.ts:8664](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8664)

___

### title

• `Optional` **title**: `string`

View title displayed in the UI.

The view title is initially taken from the extension `package.json` contribution.

#### Defined in

[index.d.ts:8649](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8649)

___

### viewType

• `Readonly` **viewType**: `string`

Identifies the type of the webview view, such as `'hexEditor.dataView'`.

#### Defined in

[index.d.ts:8637](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8637)

___

### visible

• `Readonly` **visible**: `boolean`

Tracks if the webview is currently visible.

Views are visible when they are on the screen and expanded.

#### Defined in

[index.d.ts:8671](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8671)

___

### webview

• `Readonly` **webview**: [`Webview`](codearts_plugin_.Webview.md)

The underlying webview for the view.

#### Defined in

[index.d.ts:8642](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8642)

## Methods

### show

▸ **show**(`preserveFocus?`): `void`

Reveal the view in the UI.

If the view is collapsed, this will expand it.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `preserveFocus?` | `boolean` | When `true` the view will not take focus. |

#### Returns

`void`

#### Defined in

[index.d.ts:8692](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8692)
