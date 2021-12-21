**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CustomDocumentEditEvent

# Interface: CustomDocumentEditEvent\<T>

Event triggered by extensions to signal to VS Code that an edit has occurred on an [`CustomDocument`](#CustomDocument).

**`see`** [`CustomDocumentProvider.onDidChangeCustomDocument`](#CustomDocumentProvider.onDidChangeCustomDocument).

## Type parameters

Name | Type | Default |
------ | ------ | ------ |
`T` | [CustomDocument](_index_d_._plugin_.customdocument.md) | CustomDocument |

## Hierarchy

* **CustomDocumentEditEvent**

## Index

### Properties

* [document](_index_d_._plugin_.customdocumenteditevent.md#document)
* [label](_index_d_._plugin_.customdocumenteditevent.md#label)

### Methods

* [redo](_index_d_._plugin_.customdocumenteditevent.md#redo)
* [undo](_index_d_._plugin_.customdocumenteditevent.md#undo)

## Properties

### document

• `Readonly` **document**: T

*Defined in [index.d.ts:7697](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7697)*

The document that the edit is for.

___

### label

• `Optional` `Readonly` **label**: string

*Defined in [index.d.ts:7722](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7722)*

Display name describing the edit.

This will be shown to users in the UI for undo/redo operations.

## Methods

### redo

▸ **redo**(): [Thenable](_index_d_.thenable.md)\<void> \| void

*Defined in [index.d.ts:7715](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7715)*

Redo the edit operation.

This is invoked by VS Code when the user redoes this edit. To implement `redo`, your
extension should restore the document and editor to the state they were in just after this
edit was added to VS Code's internal edit stack by `onDidChangeCustomDocument`.

**Returns:** [Thenable](_index_d_.thenable.md)\<void> \| void

___

### undo

▸ **undo**(): [Thenable](_index_d_.thenable.md)\<void> \| void

*Defined in [index.d.ts:7706](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7706)*

Undo the edit operation.

This is invoked by VS Code when the user undoes this edit. To implement `undo`, your
extension should restore the document and editor to the state they were in just before this
edit was added to VS Code's internal edit stack by `onDidChangeCustomDocument`.

**Returns:** [Thenable](_index_d_.thenable.md)\<void> \| void
