**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FoldingRangeKind

# Enumeration: FoldingRangeKind

An enumeration of specific folding range kinds. The kind is an optional field of a [FoldingRange](#FoldingRange)
and is used to distinguish specific folding ranges such as ranges originated from comments. The kind is used by commands like
`Fold all comments` or `Fold all regions`.
If the kind is not set on the range, the range originated from a syntax element other than comments, imports or region markers.

## Index

### Enumeration members

* [Comment](_index_d_._plugin_.foldingrangekind.md#comment)
* [Imports](_index_d_._plugin_.foldingrangekind.md#imports)
* [Region](_index_d_._plugin_.foldingrangekind.md#region)

## Enumeration members

### Comment

•  **Comment**:  = 1

*Defined in [index.d.ts:4456](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4456)*

Kind for folding range representing a comment.

___

### Imports

•  **Imports**:  = 2

*Defined in [index.d.ts:4460](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4460)*

Kind for folding range representing a import.

___

### Region

•  **Region**:  = 3

*Defined in [index.d.ts:4464](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4464)*

Kind for folding range representing regions originating from folding markers like `#region` and `#endregion`.
