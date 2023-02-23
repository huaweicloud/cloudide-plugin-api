[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CompletionList

# Class: CompletionList<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CompletionList

Represents a collection of [completion items](#CompletionItem) to be presented
in the editor.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CompletionItem`](cloudide_plugin_.CompletionItem.md) = [`CompletionItem`](cloudide_plugin_.CompletionItem.md) |

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.CompletionList.md#constructor)

### Properties

- [isIncomplete](cloudide_plugin_.CompletionList.md#isincomplete)
- [items](cloudide_plugin_.CompletionList.md#items)

## Constructors

### constructor

• **new CompletionList**<`T`\>(`items?`, `isIncomplete?`)

Creates a new completion list.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CompletionItem`](cloudide_plugin_.CompletionItem.md)<`T`\> = [`CompletionItem`](cloudide_plugin_.CompletionItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items?` | [`CompletionItem`](cloudide_plugin_.CompletionItem.md)[] | The completion items. |
| `isIncomplete?` | `boolean` | The list is not complete. |

#### Defined in

[index.d.ts:7620](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7620)

## Properties

### isIncomplete

• `Optional` **isIncomplete**: `boolean`

This list is not complete. Further typing should result in recomputing
this list.

#### Defined in

[index.d.ts:7607](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7607)

___

### items

• **items**: [`CompletionItem`](cloudide_plugin_.CompletionItem.md)[]

The completion items.

#### Defined in

[index.d.ts:7612](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7612)
