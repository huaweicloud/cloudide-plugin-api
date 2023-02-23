[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextDocumentContentProvider

# Interface: TextDocumentContentProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextDocumentContentProvider

A text document content provider allows to add readonly documents
to the editor, such as source from a dll or generated html from md.

Content providers are [registered](#workspace.registerTextDocumentContentProvider)
for a [uri-scheme](#Uri.scheme). When a uri with that scheme is to
be [loaded](#workspace.openTextDocument) the content provider is
asked.

## Table of contents

### Properties

- [onDidChange](cloudide_plugin_.TextDocumentContentProvider.md#ondidchange)

### Methods

- [provideTextDocumentContent](cloudide_plugin_.TextDocumentContentProvider.md#providetextdocumentcontent)

## Properties

### onDidChange

• `Optional` **onDidChange**: [`Event`](cloudide_plugin_.Event.md)<[`Uri`](../classes/cloudide_plugin_.Uri.md)\>

An event to signal a resource has changed.

#### Defined in

[index.d.ts:2134](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2134)

## Methods

### provideTextDocumentContent

▸ **provideTextDocumentContent**(`uri`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`string`\>

Provide textual content for a given uri.

The editor will use the returned string-content to create a readonly
[document](#TextDocument). Resources allocated should be released when
the corresponding document has been [closed](#workspace.onDidCloseTextDocument).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | An uri which scheme matches the scheme this provider was [registered](#workspace.registerTextDocumentContentProvider) for. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`string`\>

A string or a thenable that resolves to such.

#### Defined in

[index.d.ts:2147](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2147)
