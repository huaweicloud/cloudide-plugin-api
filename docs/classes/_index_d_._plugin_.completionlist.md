**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CompletionList

# Class: CompletionList

Represents a collection of [completion items](#CompletionItem) to be presented
in the editor.

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

\+ **new CompletionList**(`items?`: [CompletionItem](_index_d_._plugin_.completionitem.md)[], `isIncomplete?`: boolean): [CompletionList](_index_d_._plugin_.completionlist.md)

*Defined in [index.d.ts:3880](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3880)*

Creates a new completion list.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`items?` | [CompletionItem](_index_d_._plugin_.completionitem.md)[] | The completion items. |
`isIncomplete?` | boolean | The list is not complete.  |

**Returns:** [CompletionList](_index_d_._plugin_.completionlist.md)

## Properties

### isIncomplete

• `Optional` **isIncomplete**: boolean

*Defined in [index.d.ts:3875](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3875)*

This list is not complete. Further typing should result in recomputing
this list.

___

### items

•  **items**: [CompletionItem](_index_d_._plugin_.completionitem.md)[]

*Defined in [index.d.ts:3880](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3880)*

The completion items.
