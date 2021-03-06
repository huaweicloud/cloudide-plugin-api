**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextDocument

# Interface: TextDocument

Represents a text document, such as a source file. Text documents have
[lines](#TextLine) and knowledge about an underlying resource like a file.

## Hierarchy

* **TextDocument**

## Index

### Properties

* [eol](_index_d_._plugin_.textdocument.md#eol)
* [fileName](_index_d_._plugin_.textdocument.md#filename)
* [isClosed](_index_d_._plugin_.textdocument.md#isclosed)
* [isDirty](_index_d_._plugin_.textdocument.md#isdirty)
* [isUntitled](_index_d_._plugin_.textdocument.md#isuntitled)
* [languageId](_index_d_._plugin_.textdocument.md#languageid)
* [lineCount](_index_d_._plugin_.textdocument.md#linecount)
* [uri](_index_d_._plugin_.textdocument.md#uri)
* [version](_index_d_._plugin_.textdocument.md#version)

### Methods

* [getText](_index_d_._plugin_.textdocument.md#gettext)
* [getWordRangeAtPosition](_index_d_._plugin_.textdocument.md#getwordrangeatposition)
* [lineAt](_index_d_._plugin_.textdocument.md#lineat)
* [offsetAt](_index_d_._plugin_.textdocument.md#offsetat)
* [positionAt](_index_d_._plugin_.textdocument.md#positionat)
* [save](_index_d_._plugin_.textdocument.md#save)
* [validatePosition](_index_d_._plugin_.textdocument.md#validateposition)
* [validateRange](_index_d_._plugin_.textdocument.md#validaterange)

## Properties

### eol

• `Readonly` **eol**: [EndOfLine](../enums/_index_d_._plugin_.endofline.md)

*Defined in [index.d.ts:157](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L157)*

The [end of line](#EndOfLine) sequence that is predominately
used in this document.

___

### fileName

• `Readonly` **fileName**: string

*Defined in [index.d.ts:113](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L113)*

The file system path of the associated resource. Shorthand
notation for [TextDocument.uri.fsPath](#TextDocument.uri). Independent of the uri scheme.

___

### isClosed

• `Readonly` **isClosed**: boolean

*Defined in [index.d.ts:142](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L142)*

`true` if the document has been closed. A closed document isn't synchronized anymore
and won't be re-used when the same resource is opened again.

___

### isDirty

• `Readonly` **isDirty**: boolean

*Defined in [index.d.ts:136](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L136)*

`true` if there are unpersisted changes.

___

### isUntitled

• `Readonly` **isUntitled**: boolean

*Defined in [index.d.ts:120](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L120)*

Is this document representing an untitled file which has never been saved yet. *Note* that
this does not mean the document will be saved to disk, use [`uri.scheme`](#Uri.scheme)
to figure out where a document will be [saved](#FileSystemProvider), e.g. `file`, `ftp` etc.

___

### languageId

• `Readonly` **languageId**: string

*Defined in [index.d.ts:125](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L125)*

The identifier of the language associated with this document.

___

### lineCount

• `Readonly` **lineCount**: number

*Defined in [index.d.ts:162](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L162)*

The number of lines in this document.

___

### uri

• `Readonly` **uri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:107](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L107)*

The associated uri for this document.

*Note* that most documents use the `file`-scheme, which means they are files on disk. However, **not** all documents are
saved on disk and therefore the `scheme` must be checked before trying to access the underlying file or siblings on disk.

**`see`** [FileSystemProvider](#FileSystemProvider)

**`see`** [TextDocumentContentProvider](#TextDocumentContentProvider)

___

### version

• `Readonly` **version**: number

*Defined in [index.d.ts:131](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L131)*

The version number of this document (it will strictly increase after each
change, including undo/redo).

## Methods

### getText

▸ **getText**(`range?`: [Range](../classes/_index_d_._plugin_.range.md)): string

*Defined in [index.d.ts:212](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L212)*

Get the text of this document. A substring can be retrieved by providing
a range. The range will be [adjusted](#TextDocument.validateRange).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range?` | [Range](../classes/_index_d_._plugin_.range.md) | Include only the text included by the range. |

**Returns:** string

The text inside the provided range or the entire text.

___

### getWordRangeAtPosition

▸ **getWordRangeAtPosition**(`position`: [Position](../classes/_index_d_._plugin_.position.md), `regex?`: RegExp): [Range](../classes/_index_d_._plugin_.range.md) \| undefined

*Defined in [index.d.ts:232](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L232)*

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

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | A position. |
`regex?` | RegExp | Optional regular expression that describes what a word is. |

**Returns:** [Range](../classes/_index_d_._plugin_.range.md) \| undefined

A range spanning a word, or `undefined`.

___

### lineAt

▸ **lineAt**(`line`: number): [TextLine](_index_d_._plugin_.textline.md)

*Defined in [index.d.ts:172](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L172)*

Returns a text line denoted by the line number. Note
that the returned object is *not* live and changes to the
document are not reflected.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`line` | number | A line number in [0, lineCount). |

**Returns:** [TextLine](_index_d_._plugin_.textline.md)

A [line](#TextLine).

▸ **lineAt**(`position`: [Position](../classes/_index_d_._plugin_.position.md)): [TextLine](_index_d_._plugin_.textline.md)

*Defined in [index.d.ts:185](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L185)*

Returns a text line denoted by the position. Note
that the returned object is *not* live and changes to the
document are not reflected.

The position will be [adjusted](#TextDocument.validatePosition).

**`see`** [TextDocument.lineAt](#TextDocument.lineAt)

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | A position. |

**Returns:** [TextLine](_index_d_._plugin_.textline.md)

A [line](#TextLine).

___

### offsetAt

▸ **offsetAt**(`position`: [Position](../classes/_index_d_._plugin_.position.md)): number

*Defined in [index.d.ts:195](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L195)*

Converts the position to a zero-based offset.

The position will be [adjusted](#TextDocument.validatePosition).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | A position. |

**Returns:** number

A valid zero-based offset.

___

### positionAt

▸ **positionAt**(`offset`: number): [Position](../classes/_index_d_._plugin_.position.md)

*Defined in [index.d.ts:203](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L203)*

Converts a zero-based offset to a position.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`offset` | number | A zero-based offset. |

**Returns:** [Position](../classes/_index_d_._plugin_.position.md)

A valid [position](#Position).

___

### save

▸ **save**(): [Thenable](_index_d_.thenable.md)\<boolean>

*Defined in [index.d.ts:151](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L151)*

Save the underlying file.

**Returns:** [Thenable](_index_d_.thenable.md)\<boolean>

A promise that will resolve to true when the file
has been saved. If the file was not dirty or the save failed,
will return false.

___

### validatePosition

▸ **validatePosition**(`position`: [Position](../classes/_index_d_._plugin_.position.md)): [Position](../classes/_index_d_._plugin_.position.md)

*Defined in [index.d.ts:248](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L248)*

Ensure a position is contained in the range of this document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | A position. |

**Returns:** [Position](../classes/_index_d_._plugin_.position.md)

The given position or a new, adjusted position.

___

### validateRange

▸ **validateRange**(`range`: [Range](../classes/_index_d_._plugin_.range.md)): [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:240](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L240)*

Ensure a range is completely contained in this document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](../classes/_index_d_._plugin_.range.md) | A range. |

**Returns:** [Range](../classes/_index_d_._plugin_.range.md)

The given range or a new, adjusted range.
