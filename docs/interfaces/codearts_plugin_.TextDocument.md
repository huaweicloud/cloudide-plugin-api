[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextDocument

# Interface: TextDocument

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextDocument

Represents a text document, such as a source file. Text documents have
[lines](codearts_plugin_.TextLine.md) and knowledge about an underlying resource like a file.

## Table of contents

### Properties

- [eol](codearts_plugin_.TextDocument.md#eol)
- [fileName](codearts_plugin_.TextDocument.md#filename)
- [isClosed](codearts_plugin_.TextDocument.md#isclosed)
- [isDirty](codearts_plugin_.TextDocument.md#isdirty)
- [isUntitled](codearts_plugin_.TextDocument.md#isuntitled)
- [languageId](codearts_plugin_.TextDocument.md#languageid)
- [lineCount](codearts_plugin_.TextDocument.md#linecount)
- [uri](codearts_plugin_.TextDocument.md#uri)
- [version](codearts_plugin_.TextDocument.md#version)

### Methods

- [getText](codearts_plugin_.TextDocument.md#gettext)
- [getWordRangeAtPosition](codearts_plugin_.TextDocument.md#getwordrangeatposition)
- [lineAt](codearts_plugin_.TextDocument.md#lineat)
- [offsetAt](codearts_plugin_.TextDocument.md#offsetat)
- [positionAt](codearts_plugin_.TextDocument.md#positionat)
- [save](codearts_plugin_.TextDocument.md#save)
- [validatePosition](codearts_plugin_.TextDocument.md#validateposition)
- [validateRange](codearts_plugin_.TextDocument.md#validaterange)

## Properties

### eol

• `Readonly` **eol**: [`EndOfLine`](../enums/codearts_plugin_.EndOfLine.md)

The [end of line](../enums/codearts_plugin_.EndOfLine.md) sequence that is predominately
used in this document.

#### Defined in

[index.d.ts:156](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L156)

___

### fileName

• `Readonly` **fileName**: `string`

The file system path of the associated resource. Shorthand
notation for [TextDocument.uri.fsPath](codearts_plugin_.TextDocument.md#uri). Independent of the uri scheme.

#### Defined in

[index.d.ts:113](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L113)

___

### isClosed

• `Readonly` **isClosed**: `boolean`

`true` if the document has been closed. A closed document isn't synchronized anymore
and won't be re-used when the same resource is opened again.

#### Defined in

[index.d.ts:142](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L142)

___

### isDirty

• `Readonly` **isDirty**: `boolean`

`true` if there are unpersisted changes.

#### Defined in

[index.d.ts:136](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L136)

___

### isUntitled

• `Readonly` **isUntitled**: `boolean`

Is this document representing an untitled file which has never been saved yet. *Note* that
this does not mean the document will be saved to disk, use [`scheme`](../classes/codearts_plugin_.Uri.md#scheme)
to figure out where a document will be [saved](codearts_plugin_.FileSystemProvider.md), e.g. `file`, `ftp` etc.

#### Defined in

[index.d.ts:120](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L120)

___

### languageId

• `Readonly` **languageId**: `string`

The identifier of the language associated with this document.

#### Defined in

[index.d.ts:125](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L125)

___

### lineCount

• `Readonly` **lineCount**: `number`

The number of lines in this document.

#### Defined in

[index.d.ts:161](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L161)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The associated uri for this document.

*Note* that most documents use the `file`-scheme, which means they are files on disk. However, **not** all documents are
saved on disk and therefore the `scheme` must be checked before trying to access the underlying file or siblings on disk.

**`See`**

 - [FileSystemProvider](codearts_plugin_.FileSystemProvider.md)
 - [TextDocumentContentProvider](codearts_plugin_.TextDocumentContentProvider.md)

#### Defined in

[index.d.ts:107](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L107)

___

### version

• `Readonly` **version**: `number`

The version number of this document (it will strictly increase after each
change, including undo/redo).

#### Defined in

[index.d.ts:131](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L131)

## Methods

### getText

▸ **getText**(`range?`): `string`

Get the text of this document. A substring can be retrieved by providing
a range. The range will be [adjusted](codearts_plugin_.TextDocument.md#validaterange).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range?` | [`Range`](../classes/codearts_plugin_.Range.md) | Include only the text included by the range. |

#### Returns

`string`

The text inside the provided range or the entire text.

#### Defined in

[index.d.ts:212](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L212)

___

### getWordRangeAtPosition

▸ **getWordRangeAtPosition**(`position`, `regex?`): `undefined` \| [`Range`](../classes/codearts_plugin_.Range.md)

Get a word-range at the given position. By default words are defined by
common separators, like space, -, _, etc. In addition, per language custom
[word definitions} can be defined. It
is also possible to provide a custom regular expression.

* *Note 1:* A custom regular expression must not match the empty string and
if it does, it will be ignored.
* *Note 2:* A custom regular expression will fail to match multiline strings
and in the name of speed regular expressions should not match words with
spaces. Use [`text`](codearts_plugin_.TextLine.md#text) for more complex, non-wordy, scenarios.

The position will be [adjusted](codearts_plugin_.TextDocument.md#validateposition).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | A position. |
| `regex?` | `RegExp` | Optional regular expression that describes what a word is. |

#### Returns

`undefined` \| [`Range`](../classes/codearts_plugin_.Range.md)

A range spanning a word, or `undefined`.

#### Defined in

[index.d.ts:232](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L232)

___

### lineAt

▸ **lineAt**(`line`): [`TextLine`](codearts_plugin_.TextLine.md)

Returns a text line denoted by the line number. Note
that the returned object is *not* live and changes to the
document are not reflected.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `line` | `number` | A line number in [0, lineCount). |

#### Returns

[`TextLine`](codearts_plugin_.TextLine.md)

A [line](codearts_plugin_.TextLine.md).

#### Defined in

[index.d.ts:171](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L171)

▸ **lineAt**(`position`): [`TextLine`](codearts_plugin_.TextLine.md)

Returns a text line denoted by the position. Note
that the returned object is *not* live and changes to the
document are not reflected.

The position will be [adjusted](codearts_plugin_.TextDocument.md#validateposition).

**`See`**

[lineAt](codearts_plugin_.TextDocument.md#lineat)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | A position. |

#### Returns

[`TextLine`](codearts_plugin_.TextLine.md)

A [line](codearts_plugin_.TextLine.md).

#### Defined in

[index.d.ts:185](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L185)

___

### offsetAt

▸ **offsetAt**(`position`): `number`

Converts the position to a zero-based offset.

The position will be [adjusted](codearts_plugin_.TextDocument.md#validateposition).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | A position. |

#### Returns

`number`

A valid zero-based offset.

#### Defined in

[index.d.ts:195](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L195)

___

### positionAt

▸ **positionAt**(`offset`): [`Position`](../classes/codearts_plugin_.Position.md)

Converts a zero-based offset to a position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `offset` | `number` | A zero-based offset. |

#### Returns

[`Position`](../classes/codearts_plugin_.Position.md)

A valid [Position](../classes/codearts_plugin_.Position.md).

#### Defined in

[index.d.ts:203](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L203)

___

### save

▸ **save**(): [`Thenable`](Thenable.md)<`boolean`\>

Save the underlying file.

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

A promise that will resolve to `true` when the file
has been saved. If the save failed, will return `false`.

#### Defined in

[index.d.ts:150](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L150)

___

### validatePosition

▸ **validatePosition**(`position`): [`Position`](../classes/codearts_plugin_.Position.md)

Ensure a position is contained in the range of this document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | A position. |

#### Returns

[`Position`](../classes/codearts_plugin_.Position.md)

The given position or a new, adjusted position.

#### Defined in

[index.d.ts:248](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L248)

___

### validateRange

▸ **validateRange**(`range`): [`Range`](../classes/codearts_plugin_.Range.md)

Ensure a range is completely contained in this document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) | A range. |

#### Returns

[`Range`](../classes/codearts_plugin_.Range.md)

The given range or a new, adjusted range.

#### Defined in

[index.d.ts:240](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L240)
