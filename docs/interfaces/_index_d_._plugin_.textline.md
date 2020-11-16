**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextLine

# Interface: TextLine

Represents a line of text, such as a line of source code.

TextLine objects are __immutable__. When a [document](#TextDocument) changes,
previously retrieved lines will not represent the latest state.

## Hierarchy

* **TextLine**

## Index

### Properties

* [firstNonWhitespaceCharacterIndex](_index_d_._plugin_.textline.md#firstnonwhitespacecharacterindex)
* [isEmptyOrWhitespace](_index_d_._plugin_.textline.md#isemptyorwhitespace)
* [lineNumber](_index_d_._plugin_.textline.md#linenumber)
* [range](_index_d_._plugin_.textline.md#range)
* [rangeIncludingLineBreak](_index_d_._plugin_.textline.md#rangeincludinglinebreak)
* [text](_index_d_._plugin_.textline.md#text)

## Properties

### firstNonWhitespaceCharacterIndex

• `Readonly` **firstNonWhitespaceCharacterIndex**: number

*Defined in [index.d.ts:83](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L83)*

The offset of the first character which is not a whitespace character as defined
by `/\s/`. **Note** that if a line is all whitespace the length of the line is returned.

___

### isEmptyOrWhitespace

• `Readonly` **isEmptyOrWhitespace**: boolean

*Defined in [index.d.ts:89](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L89)*

Whether this line is whitespace only, shorthand
for [TextLine.firstNonWhitespaceCharacterIndex](#TextLine.firstNonWhitespaceCharacterIndex) === [TextLine.text.length](#TextLine.text).

___

### lineNumber

• `Readonly` **lineNumber**: number

*Defined in [index.d.ts:62](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L62)*

The zero-based line number.

___

### range

• `Readonly` **range**: [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:72](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L72)*

The range this line covers without the line separator characters.

___

### rangeIncludingLineBreak

• `Readonly` **rangeIncludingLineBreak**: [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:77](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L77)*

The range this line covers with the line separator characters.

___

### text

• `Readonly` **text**: string

*Defined in [index.d.ts:67](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L67)*

The text of this line without the line separator characters.
