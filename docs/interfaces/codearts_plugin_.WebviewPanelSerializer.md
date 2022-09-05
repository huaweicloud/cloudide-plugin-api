[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WebviewPanelSerializer

# Interface: WebviewPanelSerializer<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).WebviewPanelSerializer

Restore webview panels that have been persisted when vscode shuts down.

There are two types of webview persistence:

- Persistence within a session.
- Persistence across sessions (across restarts of the editor).

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

A `WebviewPanelSerializer` extends this persistence across restarts of the editor. When the editor is shutdown,
it will save off the state from `setState` of all webviews that have a serializer. When the
webview first becomes visible after the restart, this state is passed to `deserializeWebviewPanel`.
The extension can then restore the old `WebviewPanel` from this state.

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `T` | `unknown` | Type of the webview's state. |

## Table of contents

### Methods

- [deserializeWebviewPanel](codearts_plugin_.WebviewPanelSerializer.md#deserializewebviewpanel)

## Methods

### deserializeWebviewPanel

▸ **deserializeWebviewPanel**(`webviewPanel`, `state`): [`Thenable`](Thenable.md)<`void`\>

Restore a webview panel from its serialized `state`.

Called when a serialized webview first becomes visible.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `webviewPanel` | [`WebviewPanel`](codearts_plugin_.WebviewPanel.md) | Webview panel to restore. The serializer should take ownership of this panel. The serializer must restore the webview's `.html` and hook up all webview events. |
| `state` | `T` | Persisted state from the webview content. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

Thenable indicating that the webview has been fully restored.

#### Defined in

[index.d.ts:8529](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8529)
