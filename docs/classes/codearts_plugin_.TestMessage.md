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

[index.d.ts:16836](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16836)

## Properties

### actualOutput

• `Optional` **actualOutput**: `string`

Actual test output. If given with [expectedOutput](codearts_plugin_.TestMessage.md#expectedoutput), a diff view will be shown.

#### Defined in

[index.d.ts:16817](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16817)

___

### expectedOutput

• `Optional` **expectedOutput**: `string`

Expected test output. If given with [actualOutput](codearts_plugin_.TestMessage.md#actualoutput), a diff view will be shown.

#### Defined in

[index.d.ts:16812](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16812)

___

### location

• `Optional` **location**: [`Location`](codearts_plugin_.Location.md)

Associated file location.

#### Defined in

[index.d.ts:16822](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16822)

___

### message

• **message**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

Human-readable message text to display.

#### Defined in

[index.d.ts:16807](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16807)

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

[index.d.ts:16830](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16830)
