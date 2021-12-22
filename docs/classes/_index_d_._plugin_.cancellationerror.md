**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CancellationError

# Class: CancellationError

An error type that should be used to signal cancellation of an operation.

This type can be used in response to a [cancellation token](#CancellationToken)
being cancelled or when an operation is being cancelled by the
executor of that operation.

## Hierarchy

* [Error](_index_d_._plugin_.cancellationerror.md#error)

  ↳ **CancellationError**

## Index

### Constructors

* [constructor](_index_d_._plugin_.cancellationerror.md#constructor)

### Properties

* [message](_index_d_._plugin_.cancellationerror.md#message)
* [name](_index_d_._plugin_.cancellationerror.md#name)
* [stack](_index_d_._plugin_.cancellationerror.md#stack)
* [Error](_index_d_._plugin_.cancellationerror.md#error)

## Constructors

### constructor

\+ **new CancellationError**(): [CancellationError](_index_d_._plugin_.cancellationerror.md)

*Defined in [index.d.ts:1581](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1581)*

Creates a new cancellation error.

**Returns:** [CancellationError](_index_d_._plugin_.cancellationerror.md)

## Properties

### message

•  **message**: string

*Inherited from [CancellationError](_index_d_._plugin_.cancellationerror.md).[message](_index_d_._plugin_.cancellationerror.md#message)*

*Defined in node_modules/typescript/lib/lib.es5.d.ts:974*

___

### name

•  **name**: string

*Inherited from [CancellationError](_index_d_._plugin_.cancellationerror.md).[name](_index_d_._plugin_.cancellationerror.md#name)*

*Defined in node_modules/typescript/lib/lib.es5.d.ts:973*

___

### stack

• `Optional` **stack**: string

*Inherited from [CancellationError](_index_d_._plugin_.cancellationerror.md).[stack](_index_d_._plugin_.cancellationerror.md#stack)*

*Defined in node_modules/typescript/lib/lib.es5.d.ts:975*

___

### Error

▪ `Static` **Error**: ErrorConstructor

*Defined in node_modules/typescript/lib/lib.es5.d.ts:984*
