[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextLine

# Interface: TextLine

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextLine

Represents a line of text, such as a line of source code.

TextLine objects are __immutable__. When a [document](codearts_plugin_.TextDocument.md) changes,
previously retrieved lines will not represent the latest state.

## Table of contents

### Properties

- [firstNonWhitespaceCharacterIndex](codearts_plugin_.TextLine.md#firstnonwhitespacecharacterindex)
- [isEmptyOrWhitespace](codearts_plugin_.TextLine.md#isemptyorwhitespace)
- [lineNumber](codearts_plugin_.TextLine.md#linenumber)
- [range](codearts_plugin_.TextLine.md#range)
- [rangeIncludingLineBreak](codearts_plugin_.TextLine.md#rangeincludinglinebreak)
- [text](codearts_plugin_.TextLine.md#text)

## Properties

### firstNonWhitespaceCharacterIndex

• `Readonly` **firstNonWhitespaceCharacterIndex**: `number`

The offset of the first character which is not a whitespace character as defined
by `/\s/`. **Note** that if a line is all whitespace the length of the line is returned.

#### Defined in

[index.d.ts:83](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L83)

___

### isEmptyOrWhitespace

• `Readonly` **isEmptyOrWhitespace**: `boolean`

Whether this line is whitespace only, shorthand
for [firstNonWhitespaceCharacterIndex](codearts_plugin_.TextLine.md#firstnonwhitespacecharacterindex) === [TextLine.text.length](codearts_plugin_.TextLine.md#text).

#### Defined in

[index.d.ts:89](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L89)

___

### lineNumber

• `Readonly` **lineNumber**: `number`

The zero-based line number.

#### Defined in

[index.d.ts:62](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L62)

___

### range

• `Readonly` **range**: [`Range`](../classes/codearts_plugin_.Range.md)

The range this line covers without the line separator characters.

#### Defined in

[index.d.ts:72](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L72)

___

### rangeIncludingLineBreak

• `Readonly` **rangeIncludingLineBreak**: [`Range`](../classes/codearts_plugin_.Range.md)

The range this line covers with the line separator characters.

#### Defined in

[index.d.ts:77](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L77)

___

### text

• `Readonly` **text**: `string`

The text of this line without the line separator characters.

#### Defined in

[index.d.ts:67](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L67)
