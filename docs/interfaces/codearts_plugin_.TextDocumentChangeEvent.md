[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextDocumentChangeEvent

# Interface: TextDocumentChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextDocumentChangeEvent

An event describing a transactional [document](codearts_plugin_.TextDocument.md) change.

## Table of contents

### Properties

- [contentChanges](codearts_plugin_.TextDocumentChangeEvent.md#contentchanges)
- [document](codearts_plugin_.TextDocumentChangeEvent.md#document)
- [reason](codearts_plugin_.TextDocumentChangeEvent.md#reason)

## Properties

### contentChanges

• `Readonly` **contentChanges**: readonly [`TextDocumentContentChangeEvent`](codearts_plugin_.TextDocumentContentChangeEvent.md)[]

An array of content changes.

#### Defined in

[index.d.ts:11788](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L11788)

___

### document

• `Readonly` **document**: [`TextDocument`](codearts_plugin_.TextDocument.md)

The affected document.

#### Defined in

[index.d.ts:11783](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L11783)

___

### reason

• `Readonly` **reason**: `undefined` \| [`TextDocumentChangeReason`](../enums/codearts_plugin_.TextDocumentChangeReason.md)

The reason why the document was changed.
Is `undefined` if the reason is not known.

#### Defined in

[index.d.ts:11794](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L11794)
