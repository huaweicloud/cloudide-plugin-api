[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CancellationError

# Class: CancellationError

["@codearts/plugin"](../modules/_codearts_plugin_.md).CancellationError

An error type that should be used to signal cancellation of an operation.

This type can be used in response to a [cancellation token](../interfaces/codearts_plugin_.CancellationToken.md)
being cancelled or when an operation is being cancelled by the
executor of that operation.

## Hierarchy

- `Error`

  ↳ **`CancellationError`**

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CancellationError.md#constructor)

## Constructors

### constructor

• **new CancellationError**()

Creates a new cancellation error.

#### Overrides

Error.constructor

#### Defined in

[index.d.ts:1547](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1547)
