[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomTextEditorProvider

# Interface: CustomTextEditorProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomTextEditorProvider

Provider for text based custom editors.

Text based custom editors use a [`TextDocument`](codearts_plugin_.TextDocument.md) as their data model. This considerably simplifies
implementing a custom editor as it allows the editor to handle many common operations such as
undo and backup. The provider is responsible for synchronizing text changes between the webview and the `TextDocument`.

## Table of contents

### Methods

- [resolveCustomTextEditor](codearts_plugin_.CustomTextEditorProvider.md#resolvecustomtexteditor)

## Methods

### resolveCustomTextEditor

▸ **resolveCustomTextEditor**(`document`, `webviewPanel`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Resolve a custom editor for a given text resource.

This is called when a user first opens a resource for a `CustomTextEditorProvider`, or if they reopen an
existing editor using this `CustomTextEditorProvider`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | Document for the resource to resolve. |
| `webviewPanel` | [`WebviewPanel`](codearts_plugin_.WebviewPanel.md) | The webview panel used to display the editor UI for this resource.  During resolve, the provider must fill in the initial html for the content webview panel and hook up all the event listeners on it that it is interested in. The provider can also hold onto the `WebviewPanel` to use later for example in a command. See [`WebviewPanel`](codearts_plugin_.WebviewPanel.md) for additional details. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token that indicates the result is no longer needed. |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

Thenable indicating that the custom editor has been resolved.

#### Defined in

[index.d.ts:8721](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L8721)
