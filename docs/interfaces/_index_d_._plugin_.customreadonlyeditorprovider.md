**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CustomReadonlyEditorProvider

# Interface: CustomReadonlyEditorProvider\<T>

Provider for readonly custom editors that use a custom document model.

Custom editors use [`CustomDocument`](#CustomDocument) as their document model instead of a [`TextDocument`](#TextDocument).

You should use this type of custom editor when dealing with binary files or more complex scenarios. For simple
text based documents, use [`CustomTextEditorProvider`](#CustomTextEditorProvider) instead.

## Type parameters

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`T` | [CustomDocument](_index_d_._plugin_.customdocument.md) | CustomDocument | Type of the custom document returned by this provider.  |

## Hierarchy

* **CustomReadonlyEditorProvider**

  ↳ [CustomEditorProvider](_index_d_._plugin_.customeditorprovider.md)

## Index

### Methods

* [openCustomDocument](_index_d_._plugin_.customreadonlyeditorprovider.md#opencustomdocument)
* [resolveCustomEditor](_index_d_._plugin_.customreadonlyeditorprovider.md#resolvecustomeditor)

## Methods

### openCustomDocument

▸ **openCustomDocument**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `openContext`: [CustomDocumentOpenContext](_index_d_._plugin_.customdocumentopencontext.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [Thenable](_index_d_.thenable.md)\<T> \| T

*Defined in [index.d.ts:7815](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7815)*

Create a new document for a given resource.

`openCustomDocument` is called when the first time an editor for a given resource is opened. The opened
document is then passed to `resolveCustomEditor` so that the editor can be shown to the user.

Already opened `CustomDocument` are re-used if the user opened additional editors. When all editors for a
given resource are closed, the `CustomDocument` is disposed of. Opening an editor at this point will
trigger another call to `openCustomDocument`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | Uri of the document to open. |
`openContext` | [CustomDocumentOpenContext](_index_d_._plugin_.customdocumentopencontext.md) | Additional information about the opening custom document. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token that indicates the result is no longer needed.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<T> \| T

The custom document.

___

### resolveCustomEditor

▸ **resolveCustomEditor**(`document`: T, `webviewPanel`: [WebviewPanel](_index_d_._plugin_.webviewpanel.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [Thenable](_index_d_.thenable.md)\<void> \| void

*Defined in [index.d.ts:7834](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7834)*

Resolve a custom editor for a given resource.

This is called whenever the user opens a new editor for this `CustomEditorProvider`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | T | Document for the resource being resolved.  |
`webviewPanel` | [WebviewPanel](_index_d_._plugin_.webviewpanel.md) | The webview panel used to display the editor UI for this resource.  During resolve, the provider must fill in the initial html for the content webview panel and hook up all the event listeners on it that it is interested in. The provider can also hold onto the `WebviewPanel` to use later for example in a command. See [`WebviewPanel`](#WebviewPanel) for additional details.  |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token that indicates the result is no longer needed.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void> \| void

Optional thenable indicating that the custom editor has been resolved.
