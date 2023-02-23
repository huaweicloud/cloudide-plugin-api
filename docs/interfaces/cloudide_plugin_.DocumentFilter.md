[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentFilter

# Interface: DocumentFilter

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentFilter

A document filter denotes a document by different properties like
the [language](#TextDocument.languageId), the [scheme](#Uri.scheme) of
its resource, or a glob-pattern that is applied to the [path](#TextDocument.fileName).

**`Sample`**

A language filter that applies to typescript files on disk: `{ language: 'typescript', scheme: 'file' }`

**`Sample`**

A language filter that applies to all package.json paths: `{ language: 'json', scheme: 'untitled', pattern: '**​/package.json' }`

## Table of contents

### Properties

- [language](cloudide_plugin_.DocumentFilter.md#language)
- [pattern](cloudide_plugin_.DocumentFilter.md#pattern)
- [scheme](cloudide_plugin_.DocumentFilter.md#scheme)

## Properties

### language

• `Optional` **language**: `string`

A language id, like `typescript`.

#### Defined in

[index.d.ts:6552](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6552)

___

### pattern

• `Optional` **pattern**: [`GlobPattern`](../modules/_cloudide_plugin_.md#globpattern)

A [glob pattern](#GlobPattern) that is matched on the absolute path of the document. Use a [relative pattern](#RelativePattern)
to filter documents to a [workspace folder](#WorkspaceFolder).

#### Defined in

[index.d.ts:6563](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6563)

___

### scheme

• `Optional` **scheme**: `string`

A Uri [scheme](#Uri.scheme), like `file` or `untitled`.

#### Defined in

[index.d.ts:6557](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6557)
