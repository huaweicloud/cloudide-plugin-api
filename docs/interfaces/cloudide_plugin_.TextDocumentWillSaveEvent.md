[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextDocumentWillSaveEvent

# Interface: TextDocumentWillSaveEvent

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextDocumentWillSaveEvent

An event that is fired when a [document](#TextDocument) will be saved.

To make modifications to the document before it is being saved, call the
[`waitUntil`](#TextDocumentWillSaveEvent.waitUntil)-function with a thenable
that resolves to an array of [text edits](#TextEdit).

## Table of contents

### Properties

- [document](cloudide_plugin_.TextDocumentWillSaveEvent.md#document)
- [reason](cloudide_plugin_.TextDocumentWillSaveEvent.md#reason)

### Methods

- [waitUntil](cloudide_plugin_.TextDocumentWillSaveEvent.md#waituntil)

## Properties

### document

• **document**: [`TextDocument`](cloudide_plugin_.TextDocument.md)

The document that will be saved.

#### Defined in

[index.d.ts:1648](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1648)

___

### reason

• **reason**: [`TextDocumentSaveReason`](../enums/cloudide_plugin_.TextDocumentSaveReason.md)

The reason why save was triggered.

#### Defined in

[index.d.ts:1653](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1653)

## Methods

### waitUntil

▸ **waitUntil**(`thenable`): `void`

Allows to pause the event loop and to apply [pre-save-edits](#TextEdit).
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
| `thenable` | `PromiseLike`<[`TextEdit`](../classes/cloudide_plugin_.TextEdit.md)[]\> | A thenable that resolves to [pre-save-edits](#TextEdit). |

#### Returns

`void`

#### Defined in

[index.d.ts:1675](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1675)

▸ **waitUntil**(`thenable`): `void`

Allows to pause the event loop until the provided thenable resolved.

*Note:* This function can only be called during event dispatch.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | `PromiseLike`<`any`\> | A thenable that delays saving. |

#### Returns

`void`

#### Defined in

[index.d.ts:1684](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1684)
