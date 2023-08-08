[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextDocumentWillSaveEvent

# Interface: TextDocumentWillSaveEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextDocumentWillSaveEvent

An event that is fired when a [document](codearts_plugin_.TextDocument.md) will be saved.

To make modifications to the document before it is being saved, call the
[`waitUntil`](codearts_plugin_.TextDocumentWillSaveEvent.md#waituntil)-function with a thenable
that resolves to an array of [text edits](../classes/codearts_plugin_.TextEdit.md).

## Table of contents

### Properties

- [document](codearts_plugin_.TextDocumentWillSaveEvent.md#document)
- [reason](codearts_plugin_.TextDocumentWillSaveEvent.md#reason)

### Methods

- [waitUntil](codearts_plugin_.TextDocumentWillSaveEvent.md#waituntil)

## Properties

### document

• `Readonly` **document**: [`TextDocument`](codearts_plugin_.TextDocument.md)

The document that will be saved.

#### Defined in

[index.d.ts:11933](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11933)

___

### reason

• `Readonly` **reason**: [`TextDocumentSaveReason`](../enums/codearts_plugin_.TextDocumentSaveReason.md)

The reason why save was triggered.

#### Defined in

[index.d.ts:11938](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11938)

## Methods

### waitUntil

▸ **waitUntil**(`thenable`): `void`

Allows to pause the event loop and to apply [pre-save-edits](../classes/codearts_plugin_.TextEdit.md).
Edits of subsequent calls to this function will be applied in order. The
edits will be *ignored* if concurrent modifications of the document happened.

*Note:* This function can only be called during event dispatch and not
in an asynchronous manner:

```ts
workspace.onWillSaveTextDocument(event => {
	// async, will *throw* an error
	setTimeout(() => event.waitUntil(promise));

	// sync, OK
	event.waitUntil(promise);
})
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | [`Thenable`](Thenable.md)<readonly [`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\> | A thenable that resolves to [pre-save-edits](../classes/codearts_plugin_.TextEdit.md). |

#### Returns

`void`

#### Defined in

[index.d.ts:11960](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11960)

▸ **waitUntil**(`thenable`): `void`

Allows to pause the event loop until the provided thenable resolved.

*Note:* This function can only be called during event dispatch.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | [`Thenable`](Thenable.md)<`any`\> | A thenable that delays saving. |

#### Returns

`void`

#### Defined in

[index.d.ts:11969](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11969)
