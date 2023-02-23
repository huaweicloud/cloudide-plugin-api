[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextLine

# Interface: TextLine

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextLine

Represents a line of text, such as a line of source code.

TextLine objects are __immutable__. When a [document](#TextDocument) changes,
previously retrieved lines will not represent the latest state.

## Table of contents

### Properties

- [firstNonWhitespaceCharacterIndex](cloudide_plugin_.TextLine.md#firstnonwhitespacecharacterindex)
- [isEmptyOrWhitespace](cloudide_plugin_.TextLine.md#isemptyorwhitespace)
- [lineNumber](cloudide_plugin_.TextLine.md#linenumber)
- [range](cloudide_plugin_.TextLine.md#range)
- [rangeIncludingLineBreak](cloudide_plugin_.TextLine.md#rangeincludinglinebreak)
- [text](cloudide_plugin_.TextLine.md#text)

## Properties

### firstNonWhitespaceCharacterIndex

• `Readonly` **firstNonWhitespaceCharacterIndex**: `number`

The offset of the first character which is not a whitespace character as defined
by `/\s/`. **Note** that if a line is all whitespaces the length of the line is returned.

#### Defined in

[index.d.ts:1312](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1312)

___

### isEmptyOrWhitespace

• `Readonly` **isEmptyOrWhitespace**: `boolean`

Whether this line is whitespace only, shorthand
for [TextLine.firstNonWhitespaceCharacterIndex](#TextLine.firstNonWhitespaceCharacterIndex) === [TextLine.text.length](#TextLine.text).

#### Defined in

[index.d.ts:1318](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1318)

___

### lineNumber

• `Readonly` **lineNumber**: `number`

The zero-based line number.

#### Defined in

[index.d.ts:1291](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1291)

___

### range

• `Readonly` **range**: [`Range`](../classes/cloudide_plugin_.Range.md)

The range this line covers without the line separator characters.

#### Defined in

[index.d.ts:1301](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1301)

___

### rangeIncludingLineBreak

• `Readonly` **rangeIncludingLineBreak**: [`Range`](../classes/cloudide_plugin_.Range.md)

The range this line covers with the line separator characters.

#### Defined in

[index.d.ts:1306](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1306)

___

### text

• `Readonly` **text**: `string`

The text of this line without the line separator characters.

#### Defined in

[index.d.ts:1296](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1296)
