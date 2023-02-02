[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TypeHierarchyProvider

# Interface: TypeHierarchyProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).TypeHierarchyProvider

The type hierarchy provider interface describes the contract between extensions
and the type hierarchy feature.

## Table of contents

### Methods

- [prepareTypeHierarchy](codearts_plugin_.TypeHierarchyProvider.md#preparetypehierarchy)
- [provideTypeHierarchySubtypes](codearts_plugin_.TypeHierarchyProvider.md#providetypehierarchysubtypes)
- [provideTypeHierarchySupertypes](codearts_plugin_.TypeHierarchyProvider.md#providetypehierarchysupertypes)

## Methods

### prepareTypeHierarchy

▸ **prepareTypeHierarchy**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md) \| [`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

Bootstraps type hierarchy by returning the item that is denoted by the given document
and position. This item will be used as entry into the type graph. Providers should
return `undefined` or `null` when there is no item at the given location.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md) \| [`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

One or multiple type hierarchy items or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:5368](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5368)

___

### provideTypeHierarchySubtypes

▸ **provideTypeHierarchySubtypes**(`item`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

Provide all subtypes for an item, e.g all types which are derived/inherited from the given item. In
graph terms this describes directed and annotated edges inside the type graph, e.g the given item is the starting
node and the result is the nodes that can be reached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md) | The hierarchy item for which subtypes should be computed. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

A set of direct subtypes or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:5392](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5392)

___

### provideTypeHierarchySupertypes

▸ **provideTypeHierarchySupertypes**(`item`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

Provide all supertypes for an item, e.g all types from which a type is derived/inherited. In graph terms this describes directed
and annotated edges inside the type graph, e.g the given item is the starting node and the result is the nodes
that can be reached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md) | The hierarchy item for which super types should be computed. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TypeHierarchyItem`](../classes/codearts_plugin_.TypeHierarchyItem.md)[]\>

A set of direct supertypes or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:5380](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5380)
