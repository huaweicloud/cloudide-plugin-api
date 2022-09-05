[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CompletionList

# Class: CompletionList<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CompletionList

Represents a collection of [completion items](codearts_plugin_.CompletionItem.md) to be presented
in the editor.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CompletionItem`](codearts_plugin_.CompletionItem.md) = [`CompletionItem`](codearts_plugin_.CompletionItem.md) |

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CompletionList.md#constructor)

### Properties

- [isIncomplete](codearts_plugin_.CompletionList.md#isincomplete)
- [items](codearts_plugin_.CompletionList.md#items)

## Constructors

### constructor

• **new CompletionList**<`T`\>(`items?`, `isIncomplete?`)

Creates a new completion list.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CompletionItem`](codearts_plugin_.CompletionItem.md)<`T`\> = [`CompletionItem`](codearts_plugin_.CompletionItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items?` | `T`[] | The completion items. |
| `isIncomplete?` | `boolean` | The list is not complete. |

#### Defined in

[index.d.ts:4419](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L4419)

## Properties

### isIncomplete

• `Optional` **isIncomplete**: `boolean`

This list is not complete. Further typing should result in recomputing
this list.

#### Defined in

[index.d.ts:4406](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L4406)

___

### items

• **items**: `T`[]

The completion items.

#### Defined in

[index.d.ts:4411](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L4411)
