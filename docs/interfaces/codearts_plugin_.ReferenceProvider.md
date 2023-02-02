[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ReferenceProvider

# Interface: ReferenceProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).ReferenceProvider

The reference provider interface defines the contract between extensions and
the [find references](https://code.visualstudio.com/docs/editor/editingevolved#_peek)-feature.

## Table of contents

### Methods

- [provideReferences](codearts_plugin_.ReferenceProvider.md#providereferences)

## Methods

### provideReferences

▸ **provideReferences**(`document`, `position`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Location`](../classes/codearts_plugin_.Location.md)[]\>

Provide a set of project-wide references for the given position and document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the command was invoked. |
| `context` | [`ReferenceContext`](codearts_plugin_.ReferenceContext.md) | - |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Location`](../classes/codearts_plugin_.Location.md)[]\>

An array of locations or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:3368](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L3368)
