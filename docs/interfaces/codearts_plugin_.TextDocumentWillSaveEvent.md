[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextDocumentWillSaveEvent

# Interface: TextDocumentWillSaveEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextDocumentWillSaveEvent

## Table of contents

### Properties

- [document](codearts_plugin_.TextDocumentWillSaveEvent.md#document)
- [reason](codearts_plugin_.TextDocumentWillSaveEvent.md#reason)

### Methods

- [waitUntil](codearts_plugin_.TextDocumentWillSaveEvent.md#waituntil)

## Properties

### document

• `Readonly` **document**: [`TextDocument`](codearts_plugin_.TextDocument.md)

#### Defined in

[index.d.ts:11278](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11278)

___

### reason

• `Readonly` **reason**: [`TextDocumentSaveReason`](../enums/codearts_plugin_.TextDocumentSaveReason.md)

#### Defined in

[index.d.ts:11283](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11283)

## Methods

### waitUntil

▸ **waitUntil**(`thenable`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | [`Thenable`](Thenable.md)<readonly [`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\> |  |

#### Returns

`void`

#### Defined in

[index.d.ts:11305](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11305)

▸ **waitUntil**(`thenable`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | [`Thenable`](Thenable.md)<`any`\> |  |

#### Returns

`void`

#### Defined in

[index.d.ts:11314](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11314)
