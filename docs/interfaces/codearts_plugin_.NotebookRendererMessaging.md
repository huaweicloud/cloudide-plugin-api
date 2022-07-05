[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookRendererMessaging

# Interface: NotebookRendererMessaging

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookRendererMessaging

## Table of contents

### Properties

- [onDidReceiveMessage](codearts_plugin_.NotebookRendererMessaging.md#ondidreceivemessage)

### Methods

- [postMessage](codearts_plugin_.NotebookRendererMessaging.md#postmessage)

## Properties

### onDidReceiveMessage

• `Readonly` **onDidReceiveMessage**: [`Event`](codearts_plugin_.Event.md)<{ `editor`: [`NotebookEditor`](codearts_plugin_.NotebookEditor.md) ; `message`: `any`  }\>

#### Defined in

[index.d.ts:12830](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12830)

## Methods

### postMessage

▸ **postMessage**(`message`, `editor?`): [`Thenable`](Thenable.md)<`boolean`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `any` |  |
| `editor?` | [`NotebookEditor`](codearts_plugin_.NotebookEditor.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:12844](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L12844)
