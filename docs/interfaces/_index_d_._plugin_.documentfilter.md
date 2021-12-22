**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentFilter

# Interface: DocumentFilter

A document filter denotes a document by different properties like
the [language](#TextDocument.languageId), the [scheme](#Uri.scheme) of
its resource, or a glob-pattern that is applied to the [path](#TextDocument.fileName).

**`example`** <caption>A language filter that applies to typescript files on disk</caption>
{ language: 'typescript', scheme: 'file' }

**`example`** <caption>A language filter that applies to all package.json paths</caption>
{ language: 'json', scheme: 'untitled', pattern: '**​/package.json' }

## Hierarchy

* **DocumentFilter**

## Index

### Properties

* [language](_index_d_._plugin_.documentfilter.md#language)
* [pattern](_index_d_._plugin_.documentfilter.md#pattern)
* [scheme](_index_d_._plugin_.documentfilter.md#scheme)

## Properties

### language

• `Optional` `Readonly` **language**: string

*Defined in [index.d.ts:2097](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2097)*

A language id, like `typescript`.

___

### pattern

• `Optional` `Readonly` **pattern**: [GlobPattern](../modules/_index_d_._plugin_.md#globpattern)

*Defined in [index.d.ts:2108](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2108)*

A [glob pattern](#GlobPattern) that is matched on the absolute path of the document. Use a [relative pattern](#RelativePattern)
to filter documents to a [workspace folder](#WorkspaceFolder).

___

### scheme

• `Optional` `Readonly` **scheme**: string

*Defined in [index.d.ts:2102](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2102)*

A Uri [scheme](#Uri.scheme), like `file` or `untitled`.
