**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextDocumentWillSaveEvent

# Interface: TextDocumentWillSaveEvent

An event that is fired when a [document](#TextDocument) will be saved.

To make modifications to the document before it is being saved, call the
[`waitUntil`](#TextDocumentWillSaveEvent.waitUntil)-function with a thenable
that resolves to an array of [text edits](#TextEdit).

## Hierarchy

* **TextDocumentWillSaveEvent**

## Index

### Properties

* [document](_index_d_._plugin_.textdocumentwillsaveevent.md#document)
* [reason](_index_d_._plugin_.textdocumentwillsaveevent.md#reason)

### Methods

* [waitUntil](_index_d_._plugin_.textdocumentwillsaveevent.md#waituntil)

## Properties

### document

• `Readonly` **document**: [TextDocument](_index_d_._plugin_.textdocument.md)

*Defined in [index.d.ts:8683](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8683)*

The document that will be saved.

___

### reason

• `Readonly` **reason**: [TextDocumentSaveReason](../enums/_index_d_._plugin_.textdocumentsavereason.md)

*Defined in [index.d.ts:8688](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8688)*

The reason why save was triggered.

## Methods

### waitUntil

▸ **waitUntil**(`thenable`: [Thenable](_index_d_.thenable.md)\<[TextEdit](../classes/_index_d_._plugin_.textedit.md)[]>): void

*Defined in [index.d.ts:8710](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8710)*

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

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`thenable` | [Thenable](_index_d_.thenable.md)\<[TextEdit](../classes/_index_d_._plugin_.textedit.md)[]> | A thenable that resolves to [pre-save-edits](#TextEdit).  |

**Returns:** void

▸ **waitUntil**(`thenable`: [Thenable](_index_d_.thenable.md)\<any>): void

*Defined in [index.d.ts:8719](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8719)*

Allows to pause the event loop until the provided thenable resolved.

*Note:* This function can only be called during event dispatch.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`thenable` | [Thenable](_index_d_.thenable.md)\<any> | A thenable that delays saving.  |

**Returns:** void
