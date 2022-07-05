[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CompletionList

# Class: CompletionList<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CompletionList

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

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CompletionItem`](codearts_plugin_.CompletionItem.md)<`T`\> = [`CompletionItem`](codearts_plugin_.CompletionItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items?` | `T`[] |  |
| `isIncomplete?` | `boolean` |  |

#### Defined in

[index.d.ts:4419](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4419)

## Properties

### isIncomplete

• `Optional` **isIncomplete**: `boolean`

#### Defined in

[index.d.ts:4406](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4406)

___

### items

• **items**: `T`[]

#### Defined in

[index.d.ts:4411](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4411)
