[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextDocument

# Interface: TextDocument

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextDocument

Represents a text document, such as a source file. Text documents have
[lines](#TextLine) and knowledge about an underlying resource like a file.

## Table of contents

### Properties

- [eol](cloudide_plugin_.TextDocument.md#eol)
- [fileName](cloudide_plugin_.TextDocument.md#filename)
- [isClosed](cloudide_plugin_.TextDocument.md#isclosed)
- [isDirty](cloudide_plugin_.TextDocument.md#isdirty)
- [isUntitled](cloudide_plugin_.TextDocument.md#isuntitled)
- [languageId](cloudide_plugin_.TextDocument.md#languageid)
- [lineCount](cloudide_plugin_.TextDocument.md#linecount)
- [uri](cloudide_plugin_.TextDocument.md#uri)
- [version](cloudide_plugin_.TextDocument.md#version)

### Methods

- [getText](cloudide_plugin_.TextDocument.md#gettext)
- [getWordRangeAtPosition](cloudide_plugin_.TextDocument.md#getwordrangeatposition)
- [lineAt](cloudide_plugin_.TextDocument.md#lineat)
- [offsetAt](cloudide_plugin_.TextDocument.md#offsetat)
- [positionAt](cloudide_plugin_.TextDocument.md#positionat)
- [save](cloudide_plugin_.TextDocument.md#save)
- [validatePosition](cloudide_plugin_.TextDocument.md#validateposition)
- [validateRange](cloudide_plugin_.TextDocument.md#validaterange)

## Properties

### eol

• `Readonly` **eol**: [`EndOfLine`](../enums/cloudide_plugin_.EndOfLine.md)

The [end of line](#EndOfLine) sequence that is predominately
used in this document.

#### Defined in

[index.d.ts:1520](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1520)

___

### fileName

• `Readonly` **fileName**: `string`

The file system path of the associated resource. Shorthand
notation for [TextDocument.uri.fsPath](#TextDocument.uri). Independent of the uri scheme.

#### Defined in

[index.d.ts:1476](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1476)

___

### isClosed

• `Readonly` **isClosed**: `boolean`

`true` if the document have been closed. A closed document isn't synchronized anymore
and won't be re-used when the same resource is opened again.

#### Defined in

[index.d.ts:1505](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1505)

___

### isDirty

• `Readonly` **isDirty**: `boolean`

`true` if there are unpersisted changes.

#### Defined in

[index.d.ts:1499](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1499)

___

### isUntitled

• `Readonly` **isUntitled**: `boolean`

Is this document representing an untitled file which has never been saved yet. *Note* that
this does not mean the document will be saved to disk, use [`uri.scheme`](#Uri.scheme)
to figure out where a document will be [saved](#FileSystemProvider), e.g. `file`, `ftp` etc.

#### Defined in

[index.d.ts:1483](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1483)

___

### languageId

• `Readonly` **languageId**: `string`

The identifier of the language associated with this document.

#### Defined in

[index.d.ts:1488](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1488)

___

### lineCount

• `Readonly` **lineCount**: `number`

The number of lines in this document.

#### Defined in

[index.d.ts:1525](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1525)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The associated uri for this document.

*Note* that most documents use the `file`-scheme, which means they are files on disk. However, **not** all documents are
saved on disk and therefore the `scheme` must be checked before trying to access the underlying file or siblings on disk.

**`See`**

 - [FileSystemProvider](#FileSystemProvider)
 - [TextDocumentContentProvider](#TextDocumentContentProvider)

#### Defined in

[index.d.ts:1470](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1470)

___

### version

• `Readonly` **version**: `number`

The version number of this document (it will strictly increase after each
change, including undo/redo).

#### Defined in

[index.d.ts:1494](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1494)

## Methods

### getText

▸ **getText**(`range?`): `string`

Get the text of this document. A substring can be retrieved by providing
a range. The range will be [adjusted](#TextDocument.validateRange).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range?` | [`Range`](../classes/cloudide_plugin_.Range.md) | Include only the text included by the range. |

#### Returns

`string`

The text inside the provided range or the entire text.

#### Defined in

[index.d.ts:1575](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1575)

___

### getWordRangeAtPosition

▸ **getWordRangeAtPosition**(`position`, `regex?`): `undefined` \| [`Range`](../classes/cloudide_plugin_.Range.md)

Get a word-range at the given position. By default words are defined by
common separators, like space, -, _, etc. In addition, per language custom
[word definitions](#LanguageConfiguration.wordPattern) can be defined. It
is also possible to provide a custom regular expression.

* *Note 1:* A custom regular expression must not match the empty string and
if it does, it will be ignored.
* *Note 2:* A custom regular expression will fail to match multiline strings
and in the name of speed regular expressions should not match words with
spaces. Use [`TextLine.text`](#TextLine.text) for more complex, non-wordy, scenarios.

The position will be [adjusted](#TextDocument.validatePosition).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | A position. |
| `regex?` | `RegExp` | Optional regular expression that describes what a word is. |

#### Returns

`undefined` \| [`Range`](../classes/cloudide_plugin_.Range.md)

A range spanning a word, or `undefined`.

#### Defined in

[index.d.ts:1595](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1595)

___

### lineAt

▸ **lineAt**(`line`): [`TextLine`](cloudide_plugin_.TextLine.md)

Returns a text line denoted by the line number. Note
that the returned object is *not* live and changes to the
document are not reflected.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `line` | `number` | A line number in [0, lineCount). |

#### Returns

[`TextLine`](cloudide_plugin_.TextLine.md)

A [line](#TextLine).

#### Defined in

[index.d.ts:1535](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1535)

▸ **lineAt**(`position`): [`TextLine`](cloudide_plugin_.TextLine.md)

Returns a text line denoted by the position. Note
that the returned object is *not* live and changes to the
document are not reflected.

The position will be [adjusted](#TextDocument.validatePosition).

**`See`**

[TextDocument.lineAt](#TextDocument.lineAt)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | A position. |

#### Returns

[`TextLine`](cloudide_plugin_.TextLine.md)

A [line](#TextLine).

#### Defined in

[index.d.ts:1548](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1548)

___

### offsetAt

▸ **offsetAt**(`position`): `number`

Converts the position to a zero-based offset.

The position will be [adjusted](#TextDocument.validatePosition).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | A position. |

#### Returns

`number`

A valid zero-based offset.

#### Defined in

[index.d.ts:1558](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1558)

___

### positionAt

▸ **positionAt**(`offset`): [`Position`](../classes/cloudide_plugin_.Position.md)

Converts a zero-based offset to a position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `offset` | `number` | A zero-based offset. |

#### Returns

[`Position`](../classes/cloudide_plugin_.Position.md)

A valid [position](#Position).

#### Defined in

[index.d.ts:1566](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1566)

___

### save

▸ **save**(): `Promise`<`boolean`\>

Save the underlying file.

#### Returns

`Promise`<`boolean`\>

A promise that will resolve to true when the file
has been saved. If the file was not dirty or the save failed,
will return false.

#### Defined in

[index.d.ts:1514](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1514)

___

### validatePosition

▸ **validatePosition**(`position`): [`Position`](../classes/cloudide_plugin_.Position.md)

Ensure a position is contained in the range of this document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | A position. |

#### Returns

[`Position`](../classes/cloudide_plugin_.Position.md)

The given position or a new, adjusted position.

#### Defined in

[index.d.ts:1611](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1611)

___

### validateRange

▸ **validateRange**(`range`): [`Range`](../classes/cloudide_plugin_.Range.md)

Ensure a range is completely contained in this document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](../classes/cloudide_plugin_.Range.md) | A range. |

#### Returns

[`Range`](../classes/cloudide_plugin_.Range.md)

The given range or a new, adjusted range.

#### Defined in

[index.d.ts:1603](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1603)
