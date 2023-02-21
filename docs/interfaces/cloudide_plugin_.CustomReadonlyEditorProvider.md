[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CustomReadonlyEditorProvider

# Interface: CustomReadonlyEditorProvider<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CustomReadonlyEditorProvider

Provider for readonly custom editors that use a custom document model.

Custom editors use [`CustomDocument`](#CustomDocument) as their document model instead of a [`TextDocument`](#TextDocument).

You should use this type of custom editor when dealing with binary files or more complex scenarios. For simple
text based documents, use [`CustomTextEditorProvider`](#CustomTextEditorProvider) instead.

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `T` | extends [`CustomDocument`](cloudide_plugin_.CustomDocument.md) = [`CustomDocument`](cloudide_plugin_.CustomDocument.md) | Type of the custom document returned by this provider. |

## Hierarchy

- **`CustomReadonlyEditorProvider`**

  ↳ [`CustomEditorProvider`](cloudide_plugin_.CustomEditorProvider.md)

## Table of contents

### Methods

- [openCustomDocument](cloudide_plugin_.CustomReadonlyEditorProvider.md#opencustomdocument)
- [resolveCustomEditor](cloudide_plugin_.CustomReadonlyEditorProvider.md#resolvecustomeditor)

## Methods

### openCustomDocument

▸ **openCustomDocument**(`uri`, `openContext`, `token`): `T` \| [`Thenable`](Thenable.md)<`T`\>

Create a new document for a given resource.

`openCustomDocument` is called when the first time an editor for a given resource is opened. The opened
document is then passed to `resolveCustomEditor` so that the editor can be shown to the user.

Already opened `CustomDocument` are re-used if the user opened additional editors. When all editors for a
given resource are closed, the `CustomDocument` is disposed of. Opening an editor at this point will
trigger another call to `openCustomDocument`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | Uri of the document to open. |
| `openContext` | [`CustomDocumentOpenContext`](cloudide_plugin_.CustomDocumentOpenContext.md) | Additional information about the opening custom document. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token that indicates the result is no longer needed. |

#### Returns

`T` \| [`Thenable`](Thenable.md)<`T`\>

The custom document.

#### Defined in

[index.d.ts:3875](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3875)

___

### resolveCustomEditor

▸ **resolveCustomEditor**(`document`, `webviewPanel`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Resolve a custom editor for a given resource.

This is called whenever the user opens a new editor for this `CustomEditorProvider`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` | Document for the resource being resolved. |
| `webviewPanel` | [`WebviewPanel`](cloudide_plugin_.WebviewPanel.md) | The webview panel used to display the editor UI for this resource. During resolve, the provider must fill in the initial html for the content webview panel and hook up all the event listeners on it that it is interested in. The provider can also hold onto the `WebviewPanel` to use later for example in a command. See [`WebviewPanel`](#WebviewPanel) for additional details. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token that indicates the result is no longer needed. |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

Optional thenable indicating that the custom editor has been resolved.

#### Defined in

[index.d.ts:3894](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3894)
