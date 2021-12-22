**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CancellationToken

# Interface: CancellationToken

A cancellation token is passed to an asynchronous or long running
operation to request cancellation, like cancelling a request
for completion items because the user continued to type.

To get an instance of a `CancellationToken` use a
[CancellationTokenSource](#CancellationTokenSource).

## Hierarchy

* **CancellationToken**

## Index

### Properties

* [isCancellationRequested](_index_d_._plugin_.cancellationtoken.md#iscancellationrequested)
* [onCancellationRequested](_index_d_._plugin_.cancellationtoken.md#oncancellationrequested)

## Properties

### isCancellationRequested

•  **isCancellationRequested**: boolean

*Defined in [index.d.ts:1545](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1545)*

Is `true` when the token has been cancelled, `false` otherwise.

___

### onCancellationRequested

•  **onCancellationRequested**: [Event](_index_d_._plugin_.event.md)\<any>

*Defined in [index.d.ts:1550](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1550)*

An [event](#Event) which fires upon cancellation.
