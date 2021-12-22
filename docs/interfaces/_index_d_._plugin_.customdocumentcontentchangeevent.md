**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CustomDocumentContentChangeEvent

# Interface: CustomDocumentContentChangeEvent\<T>

Event triggered by extensions to signal to VS Code that the content of a [`CustomDocument`](#CustomDocument)
has changed.

**`see`** [`CustomDocumentProvider.onDidChangeCustomDocument`](#CustomDocumentProvider.onDidChangeCustomDocument).

## Type parameters

Name | Type | Default |
------ | ------ | ------ |
`T` | [CustomDocument](_index_d_._plugin_.customdocument.md) | CustomDocument |

## Hierarchy

* **CustomDocumentContentChangeEvent**

## Index

### Properties

* [document](_index_d_._plugin_.customdocumentcontentchangeevent.md#document)

## Properties

### document

• `Readonly` **document**: T

*Defined in [index.d.ts:7738](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7738)*

The document that the change is for.
