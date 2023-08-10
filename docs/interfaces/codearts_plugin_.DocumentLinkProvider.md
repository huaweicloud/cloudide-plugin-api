[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentLinkProvider

# Interface: DocumentLinkProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentLinkProvider

The document link provider defines the contract between extensions and feature of showing
links in the editor.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`DocumentLink`](../classes/codearts_plugin_.DocumentLink.md) = [`DocumentLink`](../classes/codearts_plugin_.DocumentLink.md) |

## Table of contents

### Methods

- [provideDocumentLinks](codearts_plugin_.DocumentLinkProvider.md#providedocumentlinks)
- [resolveDocumentLink](codearts_plugin_.DocumentLinkProvider.md#resolvedocumentlink)

## Methods

### provideDocumentLinks

▸ **provideDocumentLinks**(`document`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

Provide links for the given document. Note that the editor ships with a default provider that detects
`http(s)` and `file` links.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

An array of [document links](../classes/codearts_plugin_.DocumentLink.md) or a thenable that resolves to such. The lack of a result
can be signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:4768](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4768)

___

### resolveDocumentLink

▸ `Optional` **resolveDocumentLink**(`link`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

Given a link fill in its [target](../classes/codearts_plugin_.DocumentLink.md#target). This method is called when an incomplete
link is selected in the UI. Providers can implement this method and return incomplete links
(without target) from the [`provideDocumentLinks`](codearts_plugin_.DocumentLinkProvider.md#providedocumentlinks) method which
often helps to improve performance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `link` | `T` | The link that is to be resolved. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Defined in

[index.d.ts:4779](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4779)
