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

[index.d.ts:15810](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L15810)

## Properties

### actualOutput

• `Optional` **actualOutput**: `string`

#### Defined in

[index.d.ts:15791](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L15791)

___

### expectedOutput

• `Optional` **expectedOutput**: `string`

#### Defined in

[index.d.ts:15786](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L15786)

___

### location

• `Optional` **location**: [`Location`](codearts_plugin_.Location.md)

#### Defined in

[index.d.ts:15796](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L15796)

___

### message

• **message**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:15781](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L15781)

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

[index.d.ts:15804](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L15804)
