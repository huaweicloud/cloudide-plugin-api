**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Webview

# Interface: Webview

Displays html content, similarly to an iframe.

## Hierarchy

* **Webview**

## Index

### Properties

* [cspSource](_index_d_._plugin_.webview.md#cspsource)
* [html](_index_d_._plugin_.webview.md#html)
* [onDidReceiveMessage](_index_d_._plugin_.webview.md#ondidreceivemessage)
* [options](_index_d_._plugin_.webview.md#options)

### Methods

* [asWebviewUri](_index_d_._plugin_.webview.md#aswebviewuri)
* [postMessage](_index_d_._plugin_.webview.md#postmessage)

## Properties

### cspSource

• `Readonly` **cspSource**: string

*Defined in [index.d.ts:7343](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7343)*

Content security policy source for webview resources.

This is the origin that should be used in a content security policy rule:

```
img-src https: ${webview.cspSource} ...;
```

___

### html

•  **html**: string

*Defined in [index.d.ts:7300](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7300)*

HTML contents of the webview.

This should be a complete, valid html document. Changing this property causes the webview to be reloaded.

Webviews are sandboxed from normal extension process, so all communication with the webview must use
message passing. To send a message from the extension to the webview, use [`postMessage`](#Webview.postMessage).
To send message from the webview back to an extension, use the `acquireVsCodeApi` function inside the webview
to get a handle to VS Code's api and then call `.postMessage()`:

```html
<script>
    const vscode = acquireVsCodeApi(); // acquireVsCodeApi can only be invoked once
    vscode.postMessage({ message: 'hello!' });
</script>
```

To load a resources from the workspace inside a webview, use the `[asWebviewUri](#Webview.asWebviewUri)` method
and ensure the resource's directory is listed in [`WebviewOptions.localResourceRoots`](#WebviewOptions.localResourceRoots).

Keep in mind that even though webviews are sandboxed, they still allow running scripts and loading arbitrary content,
so extensions must follow all standard web security best practices when working with webviews. This includes
properly sanitizing all untrusted input (including content from the workspace) and
setting a [content security policy](https://aka.ms/vscode-api-webview-csp).

___

### onDidReceiveMessage

• `Readonly` **onDidReceiveMessage**: [Event](_index_d_._plugin_.event.md)\<any>

*Defined in [index.d.ts:7309](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7309)*

Fired when the webview content posts a message.

Webview content can post strings or json serializable objects back to a VS Code extension. They cannot
post `Blob`, `File`, `ImageData` and other DOM specific objects since the extension that receives the
message does not run in a browser environment.

___

### options

•  **options**: [WebviewOptions](_index_d_._plugin_.webviewoptions.md)

*Defined in [index.d.ts:7273](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7273)*

Content settings for the webview.

## Methods

### asWebviewUri

▸ **asWebviewUri**(`localResource`: [Uri](../classes/_index_d_._plugin_.uri.md)): [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:7332](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7332)*

Convert a uri for the local file system to one that can be used inside webviews.

Webviews cannot directly load resources from the workspace or local file system using `file:` uris. The
`asWebviewUri` function takes a local `file:` uri and converts it into a uri that can be used inside of
a webview to load the same resource:

```ts
webview.html = `<img src="${webview.asWebviewUri(vscode.Uri.file('/Users/codey/workspace/cat.gif'))}">`
```

#### Parameters:

Name | Type |
------ | ------ |
`localResource` | [Uri](../classes/_index_d_._plugin_.uri.md) |

**Returns:** [Uri](../classes/_index_d_._plugin_.uri.md)

___

### postMessage

▸ **postMessage**(`message`: any): [Thenable](_index_d_.thenable.md)\<boolean>

*Defined in [index.d.ts:7319](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7319)*

Post a message to the webview content.

Messages are only delivered if the webview is live (either visible or in the
background with `retainContextWhenHidden`).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | any | Body of the message. This must be a string or other json serializable object.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<boolean>
