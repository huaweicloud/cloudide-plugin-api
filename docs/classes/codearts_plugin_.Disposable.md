[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Disposable

# Class: Disposable

["@codearts/plugin"](../modules/_codearts_plugin_.md).Disposable

## Hierarchy

- **`Disposable`**

  ↳ [`FileSystemWatcher`](../interfaces/codearts_plugin_.FileSystemWatcher.md)

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callOnDispose` | () => `any` |  |

#### Defined in

[index.d.ts:1575](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L1575)

## Methods

### dispose

▸ **dispose**(): `any`

#### Returns

`any`

#### Defined in

[index.d.ts:1580](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L1580)

___

### from

▸ `Static` **from**(...`disposableLikes`): [`Disposable`](codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...disposableLikes` | { `dispose`: () => `any`  }[] |  |

#### Returns

[`Disposable`](codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:1565](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L1565)
