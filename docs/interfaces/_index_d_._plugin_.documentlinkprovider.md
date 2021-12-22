**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentLinkProvider

# Interface: DocumentLinkProvider\<T>

The document link provider defines the contract between extensions and feature of showing
links in the editor.

## Type parameters

Name | Type | Default |
------ | ------ | ------ |
`T` | [DocumentLink](../classes/_index_d_._plugin_.documentlink.md) | DocumentLink |

## Hierarchy

* **DocumentLinkProvider**

## Index

### Methods

* [provideDocumentLinks](_index_d_._plugin_.documentlinkprovider.md#providedocumentlinks)
* [resolveDocumentLink](_index_d_._plugin_.documentlinkprovider.md#resolvedocumentlink)

## Methods

### provideDocumentLinks

▸ **provideDocumentLinks**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

*Defined in [index.d.ts:4268](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4268)*

Provide links for the given document. Note that the editor ships with a default provider that detects
`http(s)` and `file` links.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

An array of [document links](#DocumentLink) or a thenable that resolves to such. The lack of a result
can be signaled by returning `undefined`, `null`, or an empty array.

___

### resolveDocumentLink

▸ `Optional`**resolveDocumentLink**(`link`: T, `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T>

*Defined in [index.d.ts:4279](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4279)*

Given a link fill in its [target](#DocumentLink.target). This method is called when an incomplete
link is selected in the UI. Providers can implement this method and return incomplete links
(without target) from the [`provideDocumentLinks`](#DocumentLinkProvider.provideDocumentLinks) method which
often helps to improve performance.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`link` | T | The link that is to be resolved. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token.  |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T>
