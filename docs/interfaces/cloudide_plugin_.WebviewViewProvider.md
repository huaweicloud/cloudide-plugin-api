[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / WebviewViewProvider

# Interface: WebviewViewProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).WebviewViewProvider

Provider for creating `WebviewView` elements.

## Table of contents

### Methods

- [resolveWebviewView](cloudide_plugin_.WebviewViewProvider.md#resolvewebviewview)

## Methods

### resolveWebviewView

▸ **resolveWebviewView**(`webviewView`, `context`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Revolves a webview view.

`resolveWebviewView` is called when a view first becomes visible. This may happen when the view is
first loaded or when the user hides and then shows a view again.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `webviewView` | [`WebviewView`](cloudide_plugin_.WebviewView.md) | Webview view to restore. The provider should take ownership of this view. The provider must set the webview's `.html` and hook up all webview events it is interested in. |
| `context` | `WebviewViewResolveContext` | Additional metadata about the view being resolved. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | Cancellation token indicating that the view being provided is no longer needed. |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

Optional thenable indicating that the view has been fully resolved.

#### Defined in

[index.d.ts:4120](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4120)
