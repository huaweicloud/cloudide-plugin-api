**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CallHierarchyProvider

# Interface: CallHierarchyProvider

The call hierarchy provider interface describes the contract between extensions
and the call hierarchy feature which allows to browse calls and caller of function,
methods, constructor etc.

## Hierarchy

* **CallHierarchyProvider**

## Index

### Methods

* [prepareCallHierarchy](_index_d_._plugin_.callhierarchyprovider.md#preparecallhierarchy)
* [provideCallHierarchyIncomingCalls](_index_d_._plugin_.callhierarchyprovider.md#providecallhierarchyincomingcalls)
* [provideCallHierarchyOutgoingCalls](_index_d_._plugin_.callhierarchyprovider.md#providecallhierarchyoutgoingcalls)

## Methods

### prepareCallHierarchy

▸ **prepareCallHierarchy**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[CallHierarchyItem](../classes/_index_d_._plugin_.callhierarchyitem.md) \| [CallHierarchyItem](../classes/_index_d_._plugin_.callhierarchyitem.md)[]>

*Defined in [index.d.ts:4652](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4652)*

Bootstraps call hierarchy by returning the item that is denoted by the given document
and position. This item will be used as entry into the call graph. Providers should
return `undefined` or `null` when there is no item at the given location.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[CallHierarchyItem](../classes/_index_d_._plugin_.callhierarchyitem.md) \| [CallHierarchyItem](../classes/_index_d_._plugin_.callhierarchyitem.md)[]>

A call hierarchy item or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

___

### provideCallHierarchyIncomingCalls

▸ **provideCallHierarchyIncomingCalls**(`item`: [CallHierarchyItem](../classes/_index_d_._plugin_.callhierarchyitem.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[CallHierarchyIncomingCall](../classes/_index_d_._plugin_.callhierarchyincomingcall.md)[]>

*Defined in [index.d.ts:4664](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4664)*

Provide all incoming calls for an item, e.g all callers for a method. In graph terms this describes directed
and annotated edges inside the call graph, e.g the given item is the starting node and the result is the nodes
that can be reached.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`item` | [CallHierarchyItem](../classes/_index_d_._plugin_.callhierarchyitem.md) | The hierarchy item for which incoming calls should be computed. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[CallHierarchyIncomingCall](../classes/_index_d_._plugin_.callhierarchyincomingcall.md)[]>

A set of incoming calls or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

___

### provideCallHierarchyOutgoingCalls

▸ **provideCallHierarchyOutgoingCalls**(`item`: [CallHierarchyItem](../classes/_index_d_._plugin_.callhierarchyitem.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[CallHierarchyOutgoingCall](../classes/_index_d_._plugin_.callhierarchyoutgoingcall.md)[]>

*Defined in [index.d.ts:4676](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4676)*

Provide all outgoing calls for an item, e.g call calls to functions, methods, or constructors from the given item. In
graph terms this describes directed and annotated edges inside the call graph, e.g the given item is the starting
node and the result is the nodes that can be reached.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`item` | [CallHierarchyItem](../classes/_index_d_._plugin_.callhierarchyitem.md) | The hierarchy item for which outgoing calls should be computed. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[CallHierarchyOutgoingCall](../classes/_index_d_._plugin_.callhierarchyoutgoingcall.md)[]>

A set of outgoing calls or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.
