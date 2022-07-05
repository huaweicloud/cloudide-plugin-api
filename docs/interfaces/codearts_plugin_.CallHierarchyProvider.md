[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CallHierarchyProvider

# Interface: CallHierarchyProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).CallHierarchyProvider

## Table of contents

### Methods

- [prepareCallHierarchy](codearts_plugin_.CallHierarchyProvider.md#preparecallhierarchy)
- [provideCallHierarchyIncomingCalls](codearts_plugin_.CallHierarchyProvider.md#providecallhierarchyincomingcalls)
- [provideCallHierarchyOutgoingCalls](codearts_plugin_.CallHierarchyProvider.md#providecallhierarchyoutgoingcalls)

## Methods

### prepareCallHierarchy

▸ **prepareCallHierarchy**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`CallHierarchyItem`](../classes/codearts_plugin_.CallHierarchyItem.md) \| [`CallHierarchyItem`](../classes/codearts_plugin_.CallHierarchyItem.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`CallHierarchyItem`](../classes/codearts_plugin_.CallHierarchyItem.md) \| [`CallHierarchyItem`](../classes/codearts_plugin_.CallHierarchyItem.md)[]\>

#### Defined in

[index.d.ts:5250](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L5250)

___

### provideCallHierarchyIncomingCalls

▸ **provideCallHierarchyIncomingCalls**(`item`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`CallHierarchyIncomingCall`](../classes/codearts_plugin_.CallHierarchyIncomingCall.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`CallHierarchyItem`](../classes/codearts_plugin_.CallHierarchyItem.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`CallHierarchyIncomingCall`](../classes/codearts_plugin_.CallHierarchyIncomingCall.md)[]\>

#### Defined in

[index.d.ts:5262](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L5262)

___

### provideCallHierarchyOutgoingCalls

▸ **provideCallHierarchyOutgoingCalls**(`item`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`CallHierarchyOutgoingCall`](../classes/codearts_plugin_.CallHierarchyOutgoingCall.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`CallHierarchyItem`](../classes/codearts_plugin_.CallHierarchyItem.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`CallHierarchyOutgoingCall`](../classes/codearts_plugin_.CallHierarchyOutgoingCall.md)[]\>

#### Defined in

[index.d.ts:5274](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L5274)
