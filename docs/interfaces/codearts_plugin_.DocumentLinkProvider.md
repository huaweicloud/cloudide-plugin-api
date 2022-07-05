[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentLinkProvider

# Interface: DocumentLinkProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentLinkProvider

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Defined in

[index.d.ts:4697](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L4697)

___

### resolveDocumentLink

▸ `Optional` **resolveDocumentLink**(`link`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `link` | `T` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Defined in

[index.d.ts:4708](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L4708)
