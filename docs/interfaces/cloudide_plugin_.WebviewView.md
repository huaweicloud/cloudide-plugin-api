[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / WebviewView

# Interface: WebviewView

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).WebviewView

## Table of contents

### Properties

- [description](cloudide_plugin_.WebviewView.md#description)
- [onDidChangeVisibility](cloudide_plugin_.WebviewView.md#ondidchangevisibility)
- [onDidDispose](cloudide_plugin_.WebviewView.md#ondiddispose)
- [title](cloudide_plugin_.WebviewView.md#title)
- [viewType](cloudide_plugin_.WebviewView.md#viewtype)
- [visible](cloudide_plugin_.WebviewView.md#visible)
- [webview](cloudide_plugin_.WebviewView.md#webview)

### Methods

- [show](cloudide_plugin_.WebviewView.md#show)

## Properties

### description

• `Optional` **description**: `string`

Human-readable string which is rendered less prominently in the title.

#### Defined in

[index.d.ts:4063](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4063)

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [`Event`](cloudide_plugin_.Event.md)<`boolean`\>

Event fired when the visibility of the view changes.

Actions that trigger a visibility change:

- The view is collapsed or expanded.
- The user switches to a different view group in the sidebar or panel.

Note that hiding a view using the context menu instead disposes of the view and fires `onDidDispose`.

#### Defined in

[index.d.ts:4092](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4092)

___

### onDidDispose

• `Readonly` **onDidDispose**: [`Event`](cloudide_plugin_.Event.md)<`void`\>

Event fired when the view is disposed.

Views are disposed when they are explicitly hidden by a user (this happens when a user
right clicks in a view and unchecks the webview view).

Trying to use the view after it has been disposed throws an exception.

#### Defined in

[index.d.ts:4073](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4073)

___

### title

• `Optional` **title**: `string`

View title displayed in the UI.

The view title is initially taken from the extension `package.json` contribution.

#### Defined in

[index.d.ts:4058](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4058)

___

### viewType

• `Readonly` **viewType**: `string`

Identifies the type of the webview view, such as `'hexEditor.dataView'`.

#### Defined in

[index.d.ts:4046](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4046)

___

### visible

• `Readonly` **visible**: `boolean`

Tracks if the webview is currently visible.

Views are visible when they are on the screen and expanded.

#### Defined in

[index.d.ts:4080](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4080)

___

### webview

• `Readonly` **webview**: [`Webview`](cloudide_plugin_.Webview.md)

The underlying webview for the view.

#### Defined in

[index.d.ts:4051](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4051)

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

[index.d.ts:4101](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4101)
