**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CustomTextEditorProvider

# Interface: CustomTextEditorProvider

Provider for text based custom editors.

Text based custom editors use a [`TextDocument`](#TextDocument) as their data model. This considerably simplifies
implementing a custom editor as it allows VS Code to handle many common operations such as
undo and backup. The provider is responsible for synchronizing text changes between the webview and the `TextDocument`.

## Hierarchy

* **CustomTextEditorProvider**

## Index

### Methods

* [resolveCustomTextEditor](_index_d_._plugin_.customtexteditorprovider.md#resolvecustomtexteditor)

## Methods

### resolveCustomTextEditor

▸ **resolveCustomTextEditor**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `webviewPanel`: [WebviewPanel](_index_d_._plugin_.webviewpanel.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [Thenable](_index_d_.thenable.md)\<void> \| void

*Defined in [index.d.ts:6931](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6931)*

Resolve a custom editor for a given text resource.

This is called when a user first opens a resource for a `CustomTextEditorProvider`, or if they reopen an
existing editor using this `CustomTextEditorProvider`.

To resolve a custom editor, the provider must fill in its initial html content and hook up all
the event listeners it is interested it. The provider can also hold onto the `WebviewPanel` to use later,
for example in a command. See [`WebviewPanel`](#WebviewPanel) for additional details.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | Document for the resource to resolve. |
`webviewPanel` | [WebviewPanel](_index_d_._plugin_.webviewpanel.md) | Webview to resolve. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token that indicates the result is no longer needed.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void> \| void

Thenable indicating that the custom editor has been resolved.
