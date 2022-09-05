[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WebviewPanelOptions

# Interface: WebviewPanelOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).WebviewPanelOptions

Content settings for a webview panel.

## Table of contents

### Properties

- [enableFindWidget](codearts_plugin_.WebviewPanelOptions.md#enablefindwidget)
- [retainContextWhenHidden](codearts_plugin_.WebviewPanelOptions.md#retaincontextwhenhidden)

## Properties

### enableFindWidget

• `Optional` `Readonly` **enableFindWidget**: `boolean`

Controls if the find widget is enabled in the panel.

Defaults to `false`.

#### Defined in

[index.d.ts:8354](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8354)

___

### retainContextWhenHidden

• `Optional` `Readonly` **retainContextWhenHidden**: `boolean`

Controls if the webview panel's content (iframe) is kept around even when the panel
is no longer visible.

Normally the webview panel's html context is created when the panel becomes visible
and destroyed when it is hidden. Extensions that have complex state
or UI can set the `retainContextWhenHidden` to make the editor keep the webview
context around, even when the webview moves to a background tab. When a webview using
`retainContextWhenHidden` becomes hidden, its scripts and other dynamic content are suspended.
When the panel becomes visible again, the context is automatically restored
in the exact same state it was in originally. You cannot send messages to a
hidden webview, even with `retainContextWhenHidden` enabled.

`retainContextWhenHidden` has a high memory overhead and should only be used if
your panel's context cannot be quickly saved and restored.

#### Defined in

[index.d.ts:8372](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8372)
