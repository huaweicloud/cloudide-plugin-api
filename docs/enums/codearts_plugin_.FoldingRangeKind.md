[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FoldingRangeKind

# Enumeration: FoldingRangeKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).FoldingRangeKind

An enumeration of specific folding range kinds. The kind is an optional field of a [FoldingRange](../classes/codearts_plugin_.FoldingRange.md)
and is used to distinguish specific folding ranges such as ranges originated from comments. The kind is used by commands like
`Fold all comments` or `Fold all regions`.
If the kind is not set on the range, the range originated from a syntax element other than comments, imports or region markers.

## Table of contents

### Enumeration Members

- [Comment](codearts_plugin_.FoldingRangeKind.md#comment)
- [Imports](codearts_plugin_.FoldingRangeKind.md#imports)
- [Region](codearts_plugin_.FoldingRangeKind.md#region)

## Enumeration Members

### Comment

• **Comment** = ``1``

Kind for folding range representing a comment.

#### Defined in

[index.d.ts:5074](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5074)

___

### Imports

• **Imports** = ``2``

Kind for folding range representing a import.

#### Defined in

[index.d.ts:5078](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5078)

___

### Region

• **Region** = ``3``

Kind for folding range representing regions originating from folding markers like `#region` and `#endregion`.

#### Defined in

[index.d.ts:5082](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5082)
