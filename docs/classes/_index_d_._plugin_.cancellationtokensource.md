**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CancellationTokenSource

# Class: CancellationTokenSource

A cancellation source creates and controls a [cancellation token](#CancellationToken).

## Hierarchy

* **CancellationTokenSource**

## Index

### Properties

* [token](_index_d_._plugin_.cancellationtokensource.md#token)

### Methods

* [cancel](_index_d_._plugin_.cancellationtokensource.md#cancel)
* [dispose](_index_d_._plugin_.cancellationtokensource.md#dispose)

## Properties

### token

•  **token**: [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md)

*Defined in [index.d.ts:1558](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1558)*

The cancellation token of this source.

## Methods

### cancel

▸ **cancel**(): void

*Defined in [index.d.ts:1563](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1563)*

Signal cancellation on the token.

**Returns:** void

___

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:1568](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1568)*

Dispose object and free resources.

**Returns:** void
