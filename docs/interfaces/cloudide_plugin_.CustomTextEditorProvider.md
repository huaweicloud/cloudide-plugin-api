[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CustomTextEditorProvider

# Interface: CustomTextEditorProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CustomTextEditorProvider

Provider for text based custom editors.

Text based custom editors use a [`TextDocument`](#TextDocument) as their data model. This considerably simplifies
implementing a custom editor as it allows Theia to handle many common operations such as
undo and backup. The provider is responsible for synchronizing text changes between the webview and the `TextDocument`.

## Table of contents

### Methods

- [resolveCustomTextEditor](cloudide_plugin_.CustomTextEditorProvider.md#resolvecustomtexteditor)

## Methods

### resolveCustomTextEditor

▸ **resolveCustomTextEditor**(`document`, `webviewPanel`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Resolve a custom editor for a given text resource.

This is called when a user first opens a resource for a `CustomTextEditorProvider`, or if they reopen an
existing editor using this `CustomTextEditorProvider`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | Document for the resource to resolve. |
| `webviewPanel` | [`WebviewPanel`](cloudide_plugin_.WebviewPanel.md) | The webview panel used to display the editor UI for this resource. During resolve, the provider must fill in the initial html for the content webview panel and hook up all the event listeners on it that it is interested in. The provider can also hold onto the `WebviewPanel` to use later for example in a command. See [`WebviewPanel`](#WebviewPanel) for additional details. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token that indicates the result is no longer needed. |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

Thenable indicating that the custom editor has been resolved.

#### Defined in

[index.d.ts:3759](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3759)
