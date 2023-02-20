**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextDocumentContentProvider

# Interface: TextDocumentContentProvider

A text document content provider allows to add readonly documents
to the editor, such as source from a dll or generated html from md.

Content providers are [registered](#workspace.registerTextDocumentContentProvider)
for a [uri-scheme](#Uri.scheme). When a uri with that scheme is to
be [loaded](#workspace.openTextDocument) the content provider is
asked.

## Hierarchy

* **TextDocumentContentProvider**

## Index

### Properties

* [onDidChange](_index_d_._plugin_.textdocumentcontentprovider.md#ondidchange)

### Methods

* [provideTextDocumentContent](_index_d_._plugin_.textdocumentcontentprovider.md#providetextdocumentcontent)

## Properties

### onDidChange

• `Optional` **onDidChange**: [Event](_index_d_._plugin_.event.md)\<[Uri](../classes/_index_d_._plugin_.uri.md)>

*Defined in [index.d.ts:1728](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1728)*

An event to signal a resource has changed.

## Methods

### provideTextDocumentContent

▸ **provideTextDocumentContent**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<string>

*Defined in [index.d.ts:1744](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1744)*

Provide textual content for a given uri.

The editor will use the returned string-content to create a readonly
[document](#TextDocument). Resources allocated should be released when
the corresponding document has been [closed](#workspace.onDidCloseTextDocument).

**Note**: The contents of the created [document](#TextDocument) might not be
identical to the provided text due to end-of-line-sequence normalization.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | An uri which scheme matches the scheme this provider was [registered](#workspace.registerTextDocumentContentProvider) for. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<string>

A string or a thenable that resolves to such.
