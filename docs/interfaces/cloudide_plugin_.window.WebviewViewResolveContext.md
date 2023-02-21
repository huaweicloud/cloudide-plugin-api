[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / [window](../modules/cloudide_plugin_.window.md) / WebviewViewResolveContext

# Interface: WebviewViewResolveContext<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).[window](../modules/cloudide_plugin_.window.md).WebviewViewResolveContext

Additional information the webview view being resolved.

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `T` | `unknown` | Type of the webview's state. |

## Table of contents

### Properties

- [state](cloudide_plugin_.window.WebviewViewResolveContext.md#state)

## Properties

### state

• `Readonly` **state**: `undefined` \| `T`

Persisted state from the webview content.

To save resources, VS Code normally deallocates webview documents (the iframe content) that are not visible.
For example, when the user collapse a view or switches to another top level activity in the sidebar, the
`WebviewView` itself is kept alive but the webview's underlying document is deallocated. It is recreated when
the view becomes visible again.

You can prevent this behavior by setting `retainContextWhenHidden` in the `WebviewOptions`. However this
increases resource usage and should be avoided wherever possible. Instead, you can use persisted state to
save off a webview's state so that it can be quickly recreated as needed.

To save off a persisted state, inside the webview call `acquireVsCodeApi().setState()` with
any json serializable object. To restore the state again, call `getState()`. For example:

```js
// Within the webview
const vscode = acquireVsCodeApi();

// Get existing state
const oldState = vscode.getState() || { value: 0 };

// Update state
setState({ value: oldState.value + 1 })
```

VS Code ensures that the persisted state is saved correctly when a webview is hidden and across
editor restarts.

#### Defined in

[index.d.ts:4630](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4630)
