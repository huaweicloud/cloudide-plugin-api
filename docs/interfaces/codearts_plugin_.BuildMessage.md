[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / BuildMessage

# Interface: BuildMessage

["@codearts/plugin"](../modules/_codearts_plugin_.md).BuildMessage

## Table of contents

### Properties

- [isEnd](codearts_plugin_.BuildMessage.md#isend)
- [message](codearts_plugin_.BuildMessage.md#message)

## Properties

### isEnd

• `Optional` **isEnd**: `boolean`

Whether the input build message is the last one of the current build task, the value is 'false' by default.
Please make sure that the current task must have the last message,
otherwise the current output will not be cleared when the next build task starts outputting the log.

#### Defined in

[index.d.ts:16811](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16811)

___

### message

• **message**: `string`

You can use \r\n or \n in `message` and they will be normalized to the current build output terminal.

#### Defined in

[index.d.ts:16804](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16804)
