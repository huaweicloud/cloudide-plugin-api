[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextDocumentContentProvider

# Interface: TextDocumentContentProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextDocumentContentProvider

## Table of contents

### Properties

- [onDidChange](codearts_plugin_.TextDocumentContentProvider.md#ondidchange)

### Methods

- [provideTextDocumentContent](codearts_plugin_.TextDocumentContentProvider.md#providetextdocumentcontent)

## Properties

### onDidChange

• `Optional` **onDidChange**: [`Event`](codearts_plugin_.Event.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

#### Defined in

[index.d.ts:1693](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L1693)

## Methods

### provideTextDocumentContent

▸ **provideTextDocumentContent**(`uri`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`string`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`string`\>

#### Defined in

[index.d.ts:1709](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L1709)
