**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / WebviewPanelSerializer

# Interface: WebviewPanelSerializer

Restore webview panels that have been persisted when vscode shuts down.

There are two types of webview persistence:

- Persistence within a session.
- Persistence across sessions (across restarts of VS Code).

A `WebviewPanelSerializer` is only required for the second case: persisting a webview across sessions.

Persistence within a session allows a webview to save its state when it becomes hidden
and restore its content from this state when it becomes visible again. It is powered entirely
by the webview content itself. To save off a persisted state, call `acquireVsCodeApi().setState()` with
any json serializable object. To restore the state again, call `getState()`

```js
// Within the webview
const vscode = acquireVsCodeApi();

// Get existing state
const oldState = vscode.getState() || { value: 0 };

// Update state
setState({ value: oldState.value + 1 })
```

A `WebviewPanelSerializer` extends this persistence across restarts of VS Code. When the editor is shutdown,
VS Code will save off the state from `setState` of all webviews that have a serializer. When the
webview first becomes visible after the restart, this state is passed to `deserializeWebviewPanel`.
The extension can then restore the old `WebviewPanel` from this state.

## Hierarchy

* **WebviewPanelSerializer**

## Index

### Methods

* [deserializeWebviewPanel](_index_d_._plugin_.webviewpanelserializer.md#deserializewebviewpanel)

## Methods

### deserializeWebviewPanel

▸ **deserializeWebviewPanel**(`webviewPanel`: [WebviewPanel](_index_d_._plugin_.webviewpanel.md), `state`: any): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:6903](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6903)*

Restore a webview panel from its serialized `state`.

Called when a serialized webview first becomes visible.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`webviewPanel` | [WebviewPanel](_index_d_._plugin_.webviewpanel.md) | Webview panel to restore. The serializer should take ownership of this panel. The serializer must restore the webview's `.html` and hook up all webview events. |
`state` | any | Persisted state from the webview content.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

Thenable indicating that the webview has been fully restored.
