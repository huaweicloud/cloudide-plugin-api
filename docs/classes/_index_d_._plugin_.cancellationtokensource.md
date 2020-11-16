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

*Defined in [index.d.ts:1437](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1437)*

The cancellation token of this source.

## Methods

### cancel

▸ **cancel**(): void

*Defined in [index.d.ts:1442](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1442)*

Signal cancellation on the token.

**Returns:** void

___

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:1447](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1447)*

Dispose object and free resources.

**Returns:** void
