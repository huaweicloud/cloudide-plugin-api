[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CancellationTokenSource

# Class: CancellationTokenSource

["@codearts/plugin"](../modules/_codearts_plugin_.md).CancellationTokenSource

A cancellation source creates and controls a [cancellation token](../interfaces/codearts_plugin_.CancellationToken.md).

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CancellationTokenSource.md#constructor)

### Properties

- [token](codearts_plugin_.CancellationTokenSource.md#token)

### Methods

- [cancel](codearts_plugin_.CancellationTokenSource.md#cancel)
- [dispose](codearts_plugin_.CancellationTokenSource.md#dispose)

## Constructors

### constructor

• **new CancellationTokenSource**()

## Properties

### token

• **token**: [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md)

The cancellation token of this source.

#### Defined in

[index.d.ts:1522](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1522)

## Methods

### cancel

▸ **cancel**(): `void`

Signal cancellation on the token.

#### Returns

`void`

#### Defined in

[index.d.ts:1527](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1527)

___

### dispose

▸ **dispose**(): `void`

Dispose object and free resources.

#### Returns

`void`

#### Defined in

[index.d.ts:1532](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1532)
