[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestMessage

# Class: TestMessage

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestMessage

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TestMessage.md#constructor)

### Properties

- [actualOutput](codearts_plugin_.TestMessage.md#actualoutput)
- [expectedOutput](codearts_plugin_.TestMessage.md#expectedoutput)
- [location](codearts_plugin_.TestMessage.md#location)
- [message](codearts_plugin_.TestMessage.md#message)

### Methods

- [diff](codearts_plugin_.TestMessage.md#diff)

## Constructors

### constructor

• **new TestMessage**(`message`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md) |  |

#### Defined in

[index.d.ts:15840](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15840)

## Properties

### actualOutput

• `Optional` **actualOutput**: `string`

#### Defined in

[index.d.ts:15821](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15821)

___

### expectedOutput

• `Optional` **expectedOutput**: `string`

#### Defined in

[index.d.ts:15816](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15816)

___

### location

• `Optional` **location**: [`Location`](codearts_plugin_.Location.md)

#### Defined in

[index.d.ts:15826](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15826)

___

### message

• **message**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:15811](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15811)

## Methods

### diff

▸ `Static` **diff**(`message`, `expected`, `actual`): [`TestMessage`](codearts_plugin_.TestMessage.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md) |  |
| `expected` | `string` |  |
| `actual` | `string` |  |

#### Returns

[`TestMessage`](codearts_plugin_.TestMessage.md)

#### Defined in

[index.d.ts:15834](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15834)
