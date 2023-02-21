[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Disposable

# Class: Disposable

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Disposable

## Hierarchy

- **`Disposable`**

  ↳ [`FileSystemWatcher`](../interfaces/cloudide_plugin_.FileSystemWatcher.md)

  ↳ [`TreeView`](../interfaces/cloudide_plugin_.TreeView.md)

  ↳ [`DebugAdapter`](../interfaces/cloudide_plugin_.DebugAdapter.md)

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.Disposable.md#constructor)

### Methods

- [dispose](cloudide_plugin_.Disposable.md#dispose)
- [create](cloudide_plugin_.Disposable.md#create)
- [from](cloudide_plugin_.Disposable.md#from)

## Constructors

### constructor

• **new Disposable**(`func`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `func` | () => `void` |

#### Defined in

[index.d.ts:23](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L23)

• **new Disposable**(`callOnDispose`)

Creates a new Disposable calling the provided function
on dispose.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callOnDispose` | `Function` | Function that disposes something. |

#### Defined in

[index.d.ts:47](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L47)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this object.

#### Returns

`void`

#### Defined in

[index.d.ts:27](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L27)

___

### create

▸ `Static` **create**(`func`): [`Disposable`](cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `func` | () => `void` |

#### Returns

[`Disposable`](cloudide_plugin_.Disposable.md)

#### Defined in

[index.d.ts:29](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L29)

___

### from

▸ `Static` **from**(`...disposableLikes`): [`Disposable`](cloudide_plugin_.Disposable.md)

Combine many disposable-likes into one. Use this method
when having objects with a dispose function which are not
instances of Disposable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...disposableLikes` | { `dispose`: () => `any`  }[] | Objects that have at least a `dispose`-function member. |

#### Returns

[`Disposable`](cloudide_plugin_.Disposable.md)

Returns a new disposable which, upon dispose, will
dispose all provided disposables.

#### Defined in

[index.d.ts:40](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L40)
