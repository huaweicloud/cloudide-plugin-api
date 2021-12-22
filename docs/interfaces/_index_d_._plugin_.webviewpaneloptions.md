**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / WebviewPanelOptions

# Interface: WebviewPanelOptions

Content settings for a webview panel.

## Hierarchy

* **WebviewPanelOptions**

## Index

### Properties

* [enableFindWidget](_index_d_._plugin_.webviewpaneloptions.md#enablefindwidget)
* [retainContextWhenHidden](_index_d_._plugin_.webviewpaneloptions.md#retaincontextwhenhidden)

## Properties

### enableFindWidget

• `Optional` `Readonly` **enableFindWidget**: boolean

*Defined in [index.d.ts:7355](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7355)*

Controls if the find widget is enabled in the panel.

Defaults to false.

___

### retainContextWhenHidden

• `Optional` `Readonly` **retainContextWhenHidden**: boolean

*Defined in [index.d.ts:7373](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7373)*

Controls if the webview panel's content (iframe) is kept around even when the panel
is no longer visible.

Normally the webview panel's html context is created when the panel becomes visible
and destroyed when it is hidden. Extensions that have complex state
or UI can set the `retainContextWhenHidden` to make VS Code keep the webview
context around, even when the webview moves to a background tab. When a webview using
`retainContextWhenHidden` becomes hidden, its scripts and other dynamic content are suspended.
When the panel becomes visible again, the context is automatically restored
in the exact same state it was in originally. You cannot send messages to a
hidden webview, even with `retainContextWhenHidden` enabled.

`retainContextWhenHidden` has a high memory overhead and should only be used if
your panel's context cannot be quickly saved and restored.
