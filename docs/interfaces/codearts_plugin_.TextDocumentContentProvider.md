[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextDocumentContentProvider

# Interface: TextDocumentContentProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextDocumentContentProvider

A text document content provider allows to add readonly documents
to the editor, such as source from a dll or generated html from md.

Content providers are [registered](../modules/codearts_plugin_.workspace.md#registertextdocumentcontentprovider)
for a [uri-scheme](../classes/codearts_plugin_.Uri.md#scheme). When a uri with that scheme is to
be [loaded](../modules/codearts_plugin_.workspace.md#opentextdocument) the content provider is
asked.

## Table of contents

### Properties

- [onDidChange](codearts_plugin_.TextDocumentContentProvider.md#ondidchange)

### Methods

- [provideTextDocumentContent](codearts_plugin_.TextDocumentContentProvider.md#providetextdocumentcontent)

## Properties

### onDidChange

• `Optional` **onDidChange**: [`Event`](codearts_plugin_.Event.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

An event to signal a resource has changed.

#### Defined in

[index.d.ts:1693](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1693)

## Methods

### provideTextDocumentContent

▸ **provideTextDocumentContent**(`uri`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`string`\>

Provide textual content for a given uri.

The editor will use the returned string-content to create a readonly
[document](codearts_plugin_.TextDocument.md). Resources allocated should be released when
the corresponding document has been [closed](../modules/codearts_plugin_.workspace.md#ondidclosetextdocument).

**Note**: The contents of the created [document](codearts_plugin_.TextDocument.md) might not be
identical to the provided text due to end-of-line-sequence normalization.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | An uri which scheme matches the scheme this provider was [registered](../modules/codearts_plugin_.workspace.md#registertextdocumentcontentprovider) for. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`string`\>

A string or a thenable that resolves to such.

#### Defined in

[index.d.ts:1709](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1709)
