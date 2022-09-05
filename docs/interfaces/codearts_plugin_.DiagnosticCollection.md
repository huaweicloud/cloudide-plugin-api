[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DiagnosticCollection

# Interface: DiagnosticCollection

["@codearts/plugin"](../modules/_codearts_plugin_.md).DiagnosticCollection

A diagnostics collection is a container that manages a set of
[diagnostics](../classes/codearts_plugin_.Diagnostic.md). Diagnostics are always scopes to a
diagnostics collection and a resource.

To get an instance of a `DiagnosticCollection` use
[createDiagnosticCollection](../modules/codearts_plugin_.languages.md#creatediagnosticcollection).

## Table of contents

### Properties

- [name](codearts_plugin_.DiagnosticCollection.md#name)

### Methods

- [clear](codearts_plugin_.DiagnosticCollection.md#clear)
- [delete](codearts_plugin_.DiagnosticCollection.md#delete)
- [dispose](codearts_plugin_.DiagnosticCollection.md#dispose)
- [forEach](codearts_plugin_.DiagnosticCollection.md#foreach)
- [get](codearts_plugin_.DiagnosticCollection.md#get)
- [has](codearts_plugin_.DiagnosticCollection.md#has)
- [set](codearts_plugin_.DiagnosticCollection.md#set)

## Properties

### name

• `Readonly` **name**: `string`

The name of this diagnostic collection, for instance `typescript`. Every diagnostic
from this collection will be associated with this name. Also, the task framework uses this
name when defining [problem matchers](https://code.visualstudio.com/docs/editor/tasks#_defining-a-problem-matcher).

#### Defined in

[index.d.ts:5998](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5998)

## Methods

### clear

▸ **clear**(): `void`

Remove all diagnostics from this collection. The same
as calling `#set(undefined)`;

#### Returns

`void`

#### Defined in

[index.d.ts:6033](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6033)

___

### delete

▸ **delete**(`uri`): `void`

Remove all diagnostics from this collection that belong
to the provided `uri`. The same as `#set(uri, undefined)`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | A resource identifier. |

#### Returns

`void`

#### Defined in

[index.d.ts:6027](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6027)

___

### dispose

▸ **dispose**(): `void`

Dispose and free associated resources. Calls
[clear](codearts_plugin_.DiagnosticCollection.md#clear).

#### Returns

`void`

#### Defined in

[index.d.ts:6065](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6065)

___

### forEach

▸ **forEach**(`callback`, `thisArg?`): `void`

Iterate over each entry in this collection.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`uri`: [`Uri`](../classes/codearts_plugin_.Uri.md), `diagnostics`: readonly [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[], `collection`: [`DiagnosticCollection`](codearts_plugin_.DiagnosticCollection.md)) => `any` | Function to execute for each entry. |
| `thisArg?` | `any` | The `this` context used when invoking the handler function. |

#### Returns

`void`

#### Defined in

[index.d.ts:6041](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6041)

___

### get

▸ **get**(`uri`): `undefined` \| readonly [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]

Get the diagnostics for a given resource. *Note* that you cannot
modify the diagnostics-array returned from this call.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | A resource identifier. |

#### Returns

`undefined` \| readonly [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]

An immutable array of [diagnostics](../classes/codearts_plugin_.Diagnostic.md) or `undefined`.

#### Defined in

[index.d.ts:6050](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6050)

___

### has

▸ **has**(`uri`): `boolean`

Check if this collection contains diagnostics for a
given resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | A resource identifier. |

#### Returns

`boolean`

`true` if this collection has diagnostic for the given resource.

#### Defined in

[index.d.ts:6059](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6059)

___

### set

▸ **set**(`uri`, `diagnostics`): `void`

Assign diagnostics for given resource. Will replace
existing diagnostics for that resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | A resource identifier. |
| `diagnostics` | `undefined` \| readonly [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[] | Array of diagnostics or `undefined` |

#### Returns

`void`

#### Defined in

[index.d.ts:6007](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6007)

▸ **set**(`entries`): `void`

Replace diagnostics for multiple resources in this collection.

 _Note_ that multiple tuples of the same uri will be merged, e.g
`[[file1, [d1]], [file1, [d2]]]` is equivalent to `[[file1, [d1, d2]]]`.
If a diagnostics item is `undefined` as in `[file1, undefined]`
all previous but not subsequent diagnostics are removed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `entries` | readonly [[`Uri`](../classes/codearts_plugin_.Uri.md), `undefined` \| readonly Diagnostic[]][] | An array of tuples, like `[[file1, [d1, d2]], [file2, [d3, d4, d5]]]`, or `undefined`. |

#### Returns

`void`

#### Defined in

[index.d.ts:6019](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6019)
