[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestMessage

# Class: TestMessage

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestMessage

Message associated with the test state. Can be linked to a specific
source range -- useful for assertion failures, for example.

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

Creates a new TestMessage instance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md) | The message to show to the user. |

#### Defined in

[index.d.ts:16675](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16675)

## Properties

### actualOutput

• `Optional` **actualOutput**: `string`

Actual test output. If given with [expectedOutput](codearts_plugin_.TestMessage.md#expectedoutput), a diff view will be shown.

#### Defined in

[index.d.ts:16656](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16656)

___

### expectedOutput

• `Optional` **expectedOutput**: `string`

Expected test output. If given with [actualOutput](codearts_plugin_.TestMessage.md#actualoutput), a diff view will be shown.

#### Defined in

[index.d.ts:16651](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16651)

___

### location

• `Optional` **location**: [`Location`](codearts_plugin_.Location.md)

Associated file location.

#### Defined in

[index.d.ts:16661](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16661)

___

### message

• **message**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

Human-readable message text to display.

#### Defined in

[index.d.ts:16646](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16646)

## Methods

### diff

▸ `Static` **diff**(`message`, `expected`, `actual`): [`TestMessage`](codearts_plugin_.TestMessage.md)

Creates a new TestMessage that will present as a diff in the editor.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md) | Message to display to the user. |
| `expected` | `string` | Expected output. |
| `actual` | `string` | Actual output. |

#### Returns

[`TestMessage`](codearts_plugin_.TestMessage.md)

#### Defined in

[index.d.ts:16669](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16669)
