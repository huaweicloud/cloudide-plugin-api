[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomReadonlyEditorProvider

# Interface: CustomReadonlyEditorProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomReadonlyEditorProvider

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `T` | extends [`CustomDocument`](codearts_plugin_.CustomDocument.md) = [`CustomDocument`](codearts_plugin_.CustomDocument.md) |  |

## Hierarchy

- **`CustomReadonlyEditorProvider`**

  ↳ [`CustomEditorProvider`](codearts_plugin_.CustomEditorProvider.md)

## Table of contents

### Methods

- [openCustomDocument](codearts_plugin_.CustomReadonlyEditorProvider.md#opencustomdocument)
- [resolveCustomEditor](codearts_plugin_.CustomReadonlyEditorProvider.md#resolvecustomeditor)

## Methods

### openCustomDocument

▸ **openCustomDocument**(`uri`, `openContext`, `token`): `T` \| [`Thenable`](Thenable.md)<`T`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `openContext` | [`CustomDocumentOpenContext`](codearts_plugin_.CustomDocumentOpenContext.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

`T` \| [`Thenable`](Thenable.md)<`T`\>

#### Defined in

[index.d.ts:8824](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L8824)

___

### resolveCustomEditor

▸ **resolveCustomEditor**(`document`, `webviewPanel`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` |  |
| `webviewPanel` | [`WebviewPanel`](codearts_plugin_.WebviewPanel.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8843](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L8843)
