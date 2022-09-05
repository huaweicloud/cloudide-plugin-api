[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CancellationToken

# Interface: CancellationToken

["@codearts/plugin"](../modules/_codearts_plugin_.md).CancellationToken

A cancellation token is passed to an asynchronous or long running
operation to request cancellation, like cancelling a request
for completion items because the user continued to type.

To get an instance of a `CancellationToken` use a
[CancellationTokenSource](../classes/codearts_plugin_.CancellationTokenSource.md).

## Table of contents

### Properties

- [isCancellationRequested](codearts_plugin_.CancellationToken.md#iscancellationrequested)
- [onCancellationRequested](codearts_plugin_.CancellationToken.md#oncancellationrequested)

## Properties

### isCancellationRequested

• **isCancellationRequested**: `boolean`

Is `true` when the token has been cancelled, `false` otherwise.

#### Defined in

[index.d.ts:1506](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1506)

___

### onCancellationRequested

• **onCancellationRequested**: [`Event`](codearts_plugin_.Event.md)<`any`\>

An [Event](codearts_plugin_.Event.md) which fires upon cancellation.

#### Defined in

[index.d.ts:1511](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1511)
