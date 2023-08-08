[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Disposable

# Class: Disposable

["@codearts/plugin"](../modules/_codearts_plugin_.md).Disposable

Represents a type which can release resources, such
as event listening or a timer.

## Hierarchy

- **`Disposable`**

  ↳ [`FileSystemWatcher`](../interfaces/codearts_plugin_.FileSystemWatcher.md)

  ↳ [`WebviewViewDialog`](../interfaces/codearts_plugin_.WebviewViewDialog.md)

  ↳ [`TreeView`](../interfaces/codearts_plugin_.TreeView.md)

  ↳ [`DebugAdapter`](../interfaces/codearts_plugin_.DebugAdapter.md)

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Disposable.md#constructor)

### Methods

- [dispose](codearts_plugin_.Disposable.md#dispose)
- [from](codearts_plugin_.Disposable.md#from)

## Constructors

### constructor

• **new Disposable**(`callOnDispose`)

Creates a new disposable that calls the provided function
on dispose.

*Note* that an asynchronous function is not awaited.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callOnDispose` | () => `any` | Function that disposes something. |

#### Defined in

[index.d.ts:1575](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1575)

## Methods

### dispose

▸ **dispose**(): `any`

Dispose this object.

#### Returns

`any`

#### Defined in

[index.d.ts:1580](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1580)

___

### from

▸ `Static` **from**(...`disposableLikes`): [`Disposable`](codearts_plugin_.Disposable.md)

Combine many disposable-likes into one. You can use this method when having objects with
a dispose function which aren't instances of `Disposable`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...disposableLikes` | { `dispose`: () => `any`  }[] | Objects that have at least a `dispose`-function member. Note that asynchronous dispose-functions aren't awaited. |

#### Returns

[`Disposable`](codearts_plugin_.Disposable.md)

Returns a new disposable which, upon dispose, will
dispose all provided disposables.

#### Defined in

[index.d.ts:1565](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1565)
