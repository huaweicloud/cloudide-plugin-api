**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CompletionList

# Class: CompletionList\<T>

Represents a collection of [completion items](#CompletionItem) to be presented
in the editor.

## Type parameters

Name | Type | Default |
------ | ------ | ------ |
`T` | [CompletionItem](_index_d_._plugin_.completionitem.md) | CompletionItem |

## Hierarchy

* **CompletionList**

## Index

### Constructors

* [constructor](_index_d_._plugin_.completionlist.md#constructor)

### Properties

* [isIncomplete](_index_d_._plugin_.completionlist.md#isincomplete)
* [items](_index_d_._plugin_.completionlist.md#items)

## Constructors

### constructor

\+ **new CompletionList**(`items?`: T[], `isIncomplete?`: boolean): [CompletionList](_index_d_._plugin_.completionlist.md)

*Defined in [index.d.ts:4117](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4117)*

Creates a new completion list.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`items?` | T[] | The completion items. |
`isIncomplete?` | boolean | The list is not complete.  |

**Returns:** [CompletionList](_index_d_._plugin_.completionlist.md)

## Properties

### isIncomplete

• `Optional` **isIncomplete**: boolean

*Defined in [index.d.ts:4112](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4112)*

This list is not complete. Further typing should result in recomputing
this list.

___

### items

•  **items**: T[]

*Defined in [index.d.ts:4117](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4117)*

The completion items.
