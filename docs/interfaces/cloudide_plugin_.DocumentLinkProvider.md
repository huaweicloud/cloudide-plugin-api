[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentLinkProvider

# Interface: DocumentLinkProvider<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentLinkProvider

The document link provider defines the contract between extensions and feature of showing
links in the editor.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`DocumentLink`](../classes/cloudide_plugin_.DocumentLink.md) = [`DocumentLink`](../classes/cloudide_plugin_.DocumentLink.md) |

## Table of contents

### Methods

- [provideDocumentLinks](cloudide_plugin_.DocumentLinkProvider.md#providedocumentlinks)
- [resolveDocumentLink](cloudide_plugin_.DocumentLinkProvider.md#resolvedocumentlink)

## Methods

### provideDocumentLinks

▸ **provideDocumentLinks**(`document`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

Provide links for the given document. Note that the editor ships with a default provider that detects
`http(s)` and `file` links.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

An array of [document links](#DocumentLink) or a thenable that resolves to such. The lack of a result
can be signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:8488](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8488)

___

### resolveDocumentLink

▸ `Optional` **resolveDocumentLink**(`link`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

Given a link fill in its [target](#DocumentLink.target). This method is called when an incomplete
link is selected in the UI. Providers can implement this method and return incomplete links
(without target) from the [`provideDocumentLinks`](#DocumentLinkProvider.provideDocumentLinks) method which
often helps to improve performance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `link` | `T` | The link that is to be resolved. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

#### Defined in

[index.d.ts:8499](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8499)
