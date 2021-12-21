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

*Defined in [index.d.ts:7735](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7735)*

The document that the change is for.
