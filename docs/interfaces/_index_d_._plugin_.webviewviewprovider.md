**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / WebviewViewProvider

# Interface: WebviewViewProvider

Provider for creating `WebviewView` elements.

## Hierarchy

* **WebviewViewProvider**

## Index

### Methods

* [resolveWebviewView](_index_d_._plugin_.webviewviewprovider.md#resolvewebviewview)

## Methods

### resolveWebviewView

▸ **resolveWebviewView**(`webviewView`: [WebviewView](_index_d_._plugin_.webviewview.md), `context`: [WebviewViewResolveContext](_index_d_._plugin_.webviewviewresolvecontext.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [Thenable](_index_d_.thenable.md)\<void> \| void

*Defined in [index.d.ts:7635](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7635)*

Revolves a webview view.

`resolveWebviewView` is called when a view first becomes visible. This may happen when the view is
first loaded or when the user hides and then shows a view again.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`webviewView` | [WebviewView](_index_d_._plugin_.webviewview.md) | Webview view to restore. The provider should take ownership of this view. The    provider must set the webview's `.html` and hook up all webview events it is interested in. |
`context` | [WebviewViewResolveContext](_index_d_._plugin_.webviewviewresolvecontext.md) | Additional metadata about the view being resolved. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | Cancellation token indicating that the view being provided is no longer needed.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void> \| void

Optional thenable indicating that the view has been fully resolved.
