[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Webview

# Interface: Webview

["@codearts/plugin"](../modules/_codearts_plugin_.md).Webview

## Table of contents

### Properties

- [cspSource](codearts_plugin_.Webview.md#cspsource)
- [html](codearts_plugin_.Webview.md#html)
- [onDidReceiveMessage](codearts_plugin_.Webview.md#ondidreceivemessage)
- [options](codearts_plugin_.Webview.md#options)

### Methods

- [asWebviewUri](codearts_plugin_.Webview.md#aswebviewuri)
- [postMessage](codearts_plugin_.Webview.md#postmessage)

## Properties

### cspSource

• `Readonly` **cspSource**: `string`

#### Defined in

[index.d.ts:8342](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8342)

___

### html

• **html**: `string`

#### Defined in

[index.d.ts:8276](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8276)

___

### onDidReceiveMessage

• `Readonly` **onDidReceiveMessage**: [`Event`](codearts_plugin_.Event.md)<`any`\>

#### Defined in

[index.d.ts:8285](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8285)

___

### options

• **options**: [`WebviewOptions`](codearts_plugin_.WebviewOptions.md)

#### Defined in

[index.d.ts:8249](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8249)

## Methods

### asWebviewUri

▸ **asWebviewUri**(`localResource`): [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `localResource` | [`Uri`](../classes/codearts_plugin_.Uri.md) |

#### Returns

[`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:8331](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8331)

___

### postMessage

▸ **postMessage**(`message`): [`Thenable`](Thenable.md)<`boolean`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `any` |  |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:8318](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8318)
