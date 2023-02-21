[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CallHierarchyProvider

# Interface: CallHierarchyProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CallHierarchyProvider

The call hierarchy provider interface describes the contract between extensions
and the call hierarchy feature which allows to browse calls and caller of function,
methods, constructor etc.

## Table of contents

### Methods

- [prepareCallHierarchy](cloudide_plugin_.CallHierarchyProvider.md#preparecallhierarchy)
- [provideCallHierarchyIncomingCalls](cloudide_plugin_.CallHierarchyProvider.md#providecallhierarchyincomingcalls)
- [provideCallHierarchyOutgoingCalls](cloudide_plugin_.CallHierarchyProvider.md#providecallhierarchyoutgoingcalls)

## Methods

### prepareCallHierarchy

▸ **prepareCallHierarchy**(`document`, `position`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`CallHierarchyItem`](../classes/cloudide_plugin_.CallHierarchyItem.md) \| [`CallHierarchyItem`](../classes/cloudide_plugin_.CallHierarchyItem.md)[]\>

Bootstraps call hierarchy by returning the item that is denoted by the given document
and position. This item will be used as entry into the call graph. Providers should
return `undefined` or `null` when there is no item at the given location.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`CallHierarchyItem`](../classes/cloudide_plugin_.CallHierarchyItem.md) \| [`CallHierarchyItem`](../classes/cloudide_plugin_.CallHierarchyItem.md)[]\>

A call hierarchy item or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:11253](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11253)

___

### provideCallHierarchyIncomingCalls

▸ **provideCallHierarchyIncomingCalls**(`item`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`CallHierarchyIncomingCall`](../classes/cloudide_plugin_.CallHierarchyIncomingCall.md)[]\>

Provide all incoming calls for an item, e.g all callers for a method. In graph terms this describes directed
and annotated edges inside the call graph, e.g the given item is the starting node and the result is the nodes
that can be reached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`CallHierarchyItem`](../classes/cloudide_plugin_.CallHierarchyItem.md) | The hierarchy item for which incoming calls should be computed. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`CallHierarchyIncomingCall`](../classes/cloudide_plugin_.CallHierarchyIncomingCall.md)[]\>

A set of incoming calls or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:11265](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11265)

___

### provideCallHierarchyOutgoingCalls

▸ **provideCallHierarchyOutgoingCalls**(`item`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`CallHierarchyOutgoingCall`](../classes/cloudide_plugin_.CallHierarchyOutgoingCall.md)[]\>

Provide all outgoing calls for an item, e.g call calls to functions, methods, or constructors from the given item. In
graph terms this describes directed and annotated edges inside the call graph, e.g the given item is the starting
node and the result is the nodes that can be reached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`CallHierarchyItem`](../classes/cloudide_plugin_.CallHierarchyItem.md) | The hierarchy item for which outgoing calls should be computed. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`CallHierarchyOutgoingCall`](../classes/cloudide_plugin_.CallHierarchyOutgoingCall.md)[]\>

A set of outgoing calls or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:11277](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11277)
