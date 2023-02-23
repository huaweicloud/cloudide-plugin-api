[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FoldingRangeKind

# Enumeration: FoldingRangeKind

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FoldingRangeKind

An enumeration of specific folding range kinds. The kind is an optional field of a [FoldingRange](#FoldingRange)
and is used to distinguish specific folding ranges such as ranges originated from comments. The kind is used by commands like
`Fold all comments` or `Fold all regions`.
If the kind is not set on the range, the range originated from a syntax element other than comments, imports or region markers.

## Table of contents

### Enumeration Members

- [Comment](cloudide_plugin_.FoldingRangeKind.md#comment)
- [Imports](cloudide_plugin_.FoldingRangeKind.md#imports)
- [Region](cloudide_plugin_.FoldingRangeKind.md#region)

## Enumeration Members

### Comment

• **Comment** = ``1``

Kind for folding range representing a comment.

#### Defined in

[index.d.ts:7278](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7278)

___

### Imports

• **Imports** = ``2``

Kind for folding range representing a import.

#### Defined in

[index.d.ts:7282](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7282)

___

### Region

• **Region** = ``3``

Kind for folding range representing regions originating from folding markers like `#region` and `#endregion`.

#### Defined in

[index.d.ts:7286](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7286)
