**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentFilter

# Interface: DocumentFilter

A document filter denotes a document by different properties like
the [language](#TextDocument.languageId), the [scheme](#Uri.scheme) of
its resource, or a glob-pattern that is applied to the [path](#TextDocument.fileName).

**`sample`** A language filter that applies to typescript files on disk: `{ language: 'typescript', scheme: 'file' }`

**`sample`** A language filter that applies to all package.json paths: `{ language: 'json', scheme: 'untitled', pattern: '**​/package.json' }`

## Hierarchy

* **DocumentFilter**

## Index

### Properties

* [language](_index_d_._plugin_.documentfilter.md#language)
* [pattern](_index_d_._plugin_.documentfilter.md#pattern)
* [scheme](_index_d_._plugin_.documentfilter.md#scheme)

## Properties

### language

• `Optional` **language**: string

*Defined in [index.d.ts:1923](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1923)*

A language id, like `typescript`.

___

### pattern

• `Optional` **pattern**: [GlobPattern](../modules/_index_d_._plugin_.md#globpattern)

*Defined in [index.d.ts:1934](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1934)*

A [glob pattern](#GlobPattern) that is matched on the absolute path of the document. Use a [relative pattern](#RelativePattern)
to filter documents to a [workspace folder](#WorkspaceFolder).

___

### scheme

• `Optional` **scheme**: string

*Defined in [index.d.ts:1928](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1928)*

A Uri [scheme](#Uri.scheme), like `file` or `untitled`.
