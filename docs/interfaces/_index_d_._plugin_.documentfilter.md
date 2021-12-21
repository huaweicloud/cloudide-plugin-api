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

*Defined in [index.d.ts:2094](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2094)*

A language id, like `typescript`.

___

### pattern

• `Optional` `Readonly` **pattern**: [GlobPattern](../modules/_index_d_._plugin_.md#globpattern)

*Defined in [index.d.ts:2105](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2105)*

A [glob pattern](#GlobPattern) that is matched on the absolute path of the document. Use a [relative pattern](#RelativePattern)
to filter documents to a [workspace folder](#WorkspaceFolder).

___

### scheme

• `Optional` `Readonly` **scheme**: string

*Defined in [index.d.ts:2099](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2099)*

A Uri [scheme](#Uri.scheme), like `file` or `untitled`.
