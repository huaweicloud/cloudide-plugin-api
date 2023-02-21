[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Webview

# Interface: Webview

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Webview

A webview displays html content, like an iframe.

## Table of contents

### Properties

- [cspSource](cloudide_plugin_.Webview.md#cspsource)
- [html](cloudide_plugin_.Webview.md#html)
- [onDidReceiveMessage](cloudide_plugin_.Webview.md#ondidreceivemessage)
- [options](cloudide_plugin_.Webview.md#options)

### Methods

- [asWebviewUri](cloudide_plugin_.Webview.md#aswebviewuri)
- [postMessage](cloudide_plugin_.Webview.md#postmessage)

## Properties

### cspSource

• `Readonly` **cspSource**: `string`

Content security policy source for webview resources.

This is the origin that should be used in a content security policy rule:

```
img-src https: ${webview.cspSource} ...;
```

#### Defined in

[index.d.ts:3466](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3466)

___

### html

• **html**: `string`

Contents of the webview.

Should be a complete html document.

#### Defined in

[index.d.ts:3428](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3428)

___

### onDidReceiveMessage

• `Readonly` **onDidReceiveMessage**: [`Event`](cloudide_plugin_.Event.md)<`any`\>

Fired when the webview content posts a message.

#### Defined in

[index.d.ts:3433](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3433)

___

### options

• **options**: [`WebviewOptions`](cloudide_plugin_.WebviewOptions.md)

Content settings for the webview.

#### Defined in

[index.d.ts:3421](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3421)

## Methods

### asWebviewUri

▸ **asWebviewUri**(`localResource`): [`Uri`](../classes/cloudide_plugin_.Uri.md)

Convert a uri for the local file system to one that can be used inside webviews.

Webviews cannot directly load resources from the workspace or local file system using `file:` uris. The
`asWebviewUri` function takes a local `file:` uri and converts it into a uri that can be used inside of
a webview to load the same resource:

```ts
webview.html = `<img src="${webview.asWebviewUri(vscode.Uri.file('/Users/codey/workspace/cat.gif'))}">`
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `localResource` | [`Uri`](../classes/cloudide_plugin_.Uri.md) |

#### Returns

[`Uri`](../classes/cloudide_plugin_.Uri.md)

#### Defined in

[index.d.ts:3455](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3455)

___

### postMessage

▸ **postMessage**(`message`): `PromiseLike`<`boolean`\>

Post a message to the webview content.

Messages are only delivered if the webview is visible.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `any` | Body of the message. |

#### Returns

`PromiseLike`<`boolean`\>

#### Defined in

[index.d.ts:3442](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3442)
