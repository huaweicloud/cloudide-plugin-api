[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomEditorProvider

# Interface: CustomEditorProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomEditorProvider

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `T` | extends [`CustomDocument`](codearts_plugin_.CustomDocument.md) = [`CustomDocument`](codearts_plugin_.CustomDocument.md) |  |

## Hierarchy

- [`CustomReadonlyEditorProvider`](codearts_plugin_.CustomReadonlyEditorProvider.md)<`T`\>

  ↳ **`CustomEditorProvider`**

## Table of contents

### Properties

- [onDidChangeCustomDocument](codearts_plugin_.CustomEditorProvider.md#ondidchangecustomdocument)

### Methods

- [backupCustomDocument](codearts_plugin_.CustomEditorProvider.md#backupcustomdocument)
- [openCustomDocument](codearts_plugin_.CustomEditorProvider.md#opencustomdocument)
- [resolveCustomEditor](codearts_plugin_.CustomEditorProvider.md#resolvecustomeditor)
- [revertCustomDocument](codearts_plugin_.CustomEditorProvider.md#revertcustomdocument)
- [saveCustomDocument](codearts_plugin_.CustomEditorProvider.md#savecustomdocument)
- [saveCustomDocumentAs](codearts_plugin_.CustomEditorProvider.md#savecustomdocumentas)

## Properties

### onDidChangeCustomDocument

• `Readonly` **onDidChangeCustomDocument**: [`Event`](codearts_plugin_.Event.md)<[`CustomDocumentEditEvent`](codearts_plugin_.CustomDocumentEditEvent.md)<`T`\>\> \| [`Event`](codearts_plugin_.Event.md)<[`CustomDocumentContentChangeEvent`](codearts_plugin_.CustomDocumentContentChangeEvent.md)<`T`\>\>

#### Defined in

[index.d.ts:8878](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L8878)

## Methods

### backupCustomDocument

▸ **backupCustomDocument**(`document`, `context`, `cancellation`): [`Thenable`](Thenable.md)<[`CustomDocumentBackup`](codearts_plugin_.CustomDocumentBackup.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` |  |
| `context` | [`CustomDocumentBackupContext`](codearts_plugin_.CustomDocumentBackupContext.md) |  |
| `cancellation` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`Thenable`](Thenable.md)<[`CustomDocumentBackup`](codearts_plugin_.CustomDocumentBackup.md)\>

#### Defined in

[index.d.ts:8951](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L8951)

___

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

#### Inherited from

[CustomReadonlyEditorProvider](codearts_plugin_.CustomReadonlyEditorProvider.md).[openCustomDocument](codearts_plugin_.CustomReadonlyEditorProvider.md#opencustomdocument)

#### Defined in

[index.d.ts:8824](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L8824)

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

#### Inherited from

[CustomReadonlyEditorProvider](codearts_plugin_.CustomReadonlyEditorProvider.md).[resolveCustomEditor](codearts_plugin_.CustomReadonlyEditorProvider.md#resolvecustomeditor)

#### Defined in

[index.d.ts:8843](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L8843)

___

### revertCustomDocument

▸ **revertCustomDocument**(`document`, `cancellation`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` |  |
| `cancellation` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8928](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L8928)

___

### saveCustomDocument

▸ **saveCustomDocument**(`document`, `cancellation`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` |  |
| `cancellation` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8895](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L8895)

___

### saveCustomDocumentAs

▸ **saveCustomDocumentAs**(`document`, `destination`, `cancellation`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` |  |
| `destination` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `cancellation` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8911](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L8911)
