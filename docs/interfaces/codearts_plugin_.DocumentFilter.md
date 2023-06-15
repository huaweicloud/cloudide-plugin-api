[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentFilter

# Interface: DocumentFilter

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentFilter

A document filter denotes a document by different properties like
the [language](codearts_plugin_.TextDocument.md#languageid), the [scheme](../classes/codearts_plugin_.Uri.md#scheme) of
its resource, or a glob-pattern that is applied to the [path](codearts_plugin_.TextDocument.md#filename).

**`Example`**

A language filter that applies to typescript files on disk
```ts
{ language: 'typescript', scheme: 'file' }
```

**`Example`**

A language filter that applies to all package.json paths
```ts
{ language: 'json', pattern: '**​/package.json' }
```

## Table of contents

### Properties

- [language](codearts_plugin_.DocumentFilter.md#language)
- [notebookType](codearts_plugin_.DocumentFilter.md#notebooktype)
- [pattern](codearts_plugin_.DocumentFilter.md#pattern)
- [scheme](codearts_plugin_.DocumentFilter.md#scheme)

## Properties

### language

• `Optional` `Readonly` **language**: `string`

A language id, like `typescript`.

#### Defined in

[index.d.ts:2162](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L2162)

___

### notebookType

• `Optional` `Readonly` **notebookType**: `string`

The [type](codearts_plugin_.NotebookDocument.md#notebooktype) of a notebook, like `jupyter-notebook`. This allows
to narrow down on the type of a notebook that a [cell document](codearts_plugin_.NotebookCell.md#document) belongs to.

*Note* that setting the `notebookType`-property changes how `scheme` and `pattern` are interpreted. When set
they are evaluated against the [notebook uri](codearts_plugin_.NotebookDocument.md#uri), not the document uri.

**`Example`**

<caption>Match python document inside jupyter notebook that aren't stored yet (`untitled`)</caption>
{ language: 'python', notebookType: 'jupyter-notebook', scheme: 'untitled' }

#### Defined in

[index.d.ts:2174](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L2174)

___

### pattern

• `Optional` `Readonly` **pattern**: [`GlobPattern`](../modules/_codearts_plugin_.md#globpattern)

A [glob pattern](../modules/_codearts_plugin_.md#globpattern) that is matched on the absolute path of the document. Use a [relative pattern](../classes/codearts_plugin_.RelativePattern.md)
to filter documents to a [workspace folder](codearts_plugin_.WorkspaceFolder.md).

#### Defined in

[index.d.ts:2185](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L2185)

___

### scheme

• `Optional` `Readonly` **scheme**: `string`

A Uri [scheme](../classes/codearts_plugin_.Uri.md#scheme), like `file` or `untitled`.

#### Defined in

[index.d.ts:2179](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L2179)
