[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ImplementationProvider

# Interface: ImplementationProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).ImplementationProvider

The implementation provider interface defines the contract between extensions and
the go to implementation feature.

## Table of contents

### Methods

- [provideImplementation](codearts_plugin_.ImplementationProvider.md#provideimplementation)

## Methods

### provideImplementation

▸ **provideImplementation**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Definition`](../modules/_codearts_plugin_.md#definition) \| [`LocationLink`](codearts_plugin_.LocationLink.md)[]\>

Provide the implementations of the symbol at the given position and document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Definition`](../modules/_codearts_plugin_.md#definition) \| [`LocationLink`](codearts_plugin_.LocationLink.md)[]\>

A definition or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:2689](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L2689)
