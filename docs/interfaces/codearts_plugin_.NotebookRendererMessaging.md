[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookRendererMessaging

# Interface: NotebookRendererMessaging

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookRendererMessaging

Renderer messaging is used to communicate with a single renderer. It's returned from [createRendererMessaging](../modules/codearts_plugin_.notebooks.md#createrenderermessaging).

## Table of contents

### Properties

- [onDidReceiveMessage](codearts_plugin_.NotebookRendererMessaging.md#ondidreceivemessage)

### Methods

- [postMessage](codearts_plugin_.NotebookRendererMessaging.md#postmessage)

## Properties

### onDidReceiveMessage

• `Readonly` **onDidReceiveMessage**: [`Event`](codearts_plugin_.Event.md)<{ `editor`: [`NotebookEditor`](codearts_plugin_.NotebookEditor.md) ; `message`: `any`  }\>

An event that fires when a message is received from a renderer.

#### Defined in

[index.d.ts:13824](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13824)

## Methods

### postMessage

▸ **postMessage**(`message`, `editor?`): [`Thenable`](Thenable.md)<`boolean`\>

Send a message to one or all renderer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `any` | Message to send |
| `editor?` | [`NotebookEditor`](codearts_plugin_.NotebookEditor.md) | Editor to target with the message. If not provided, the message is sent to all renderers. |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

a boolean indicating whether the message was successfully
delivered to any renderer.

#### Defined in

[index.d.ts:13838](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13838)
