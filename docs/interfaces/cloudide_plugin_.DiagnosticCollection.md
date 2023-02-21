[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DiagnosticCollection

# Interface: DiagnosticCollection

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DiagnosticCollection

## Table of contents

### Properties

- [name](cloudide_plugin_.DiagnosticCollection.md#name)

### Methods

- [clear](cloudide_plugin_.DiagnosticCollection.md#clear)
- [delete](cloudide_plugin_.DiagnosticCollection.md#delete)
- [dispose](cloudide_plugin_.DiagnosticCollection.md#dispose)
- [forEach](cloudide_plugin_.DiagnosticCollection.md#foreach)
- [get](cloudide_plugin_.DiagnosticCollection.md#get)
- [has](cloudide_plugin_.DiagnosticCollection.md#has)
- [set](cloudide_plugin_.DiagnosticCollection.md#set)

## Properties

### name

• `Readonly` **name**: `string`

The name of this diagnostic collection, for instance `typescript`. Every diagnostic
from this collection will be associated with this name. Also, the task framework uses this
name when defining [problem matchers](https://code.visualstudio.com/docs/editor/tasks#_defining-a-problem-matcher).

#### Defined in

[index.d.ts:7853](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7853)

## Methods

### clear

▸ **clear**(): `void`

Remove all diagnostics from this collection. The same
as calling `#set(undefined)`;

#### Returns

`void`

#### Defined in

[index.d.ts:7888](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7888)

___

### delete

▸ **delete**(`uri`): `void`

Remove all diagnostics from this collection that belong
to the provided `uri`. The same as `#set(uri, undefined)`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | A resource identifier. |

#### Returns

`void`

#### Defined in

[index.d.ts:7882](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7882)

___

### dispose

▸ **dispose**(): `void`

Dispose and free associated resources. Calls
[clear](#DiagnosticCollection.clear).

#### Returns

`void`

#### Defined in

[index.d.ts:7920](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7920)

___

### forEach

▸ **forEach**(`callback`, `thisArg?`): `void`

Iterate over each entry in this collection.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`uri`: [`Uri`](../classes/cloudide_plugin_.Uri.md), `diagnostics`: [`Diagnostic`](../classes/cloudide_plugin_.Diagnostic.md)[], `collection`: [`DiagnosticCollection`](cloudide_plugin_.DiagnosticCollection.md)) => `any` | Function to execute for each entry. |
| `thisArg?` | `any` | The `this` context used when invoking the handler function. |

#### Returns

`void`

#### Defined in

[index.d.ts:7896](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7896)

___

### get

▸ **get**(`uri`): `undefined` \| [`Diagnostic`](../classes/cloudide_plugin_.Diagnostic.md)[]

Get the diagnostics for a given resource. *Note* that you cannot
modify the diagnostics-array returned from this call.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | A resource identifier. |

#### Returns

`undefined` \| [`Diagnostic`](../classes/cloudide_plugin_.Diagnostic.md)[]

An immutable array of [diagnostics](#Diagnostic) or `undefined`.

#### Defined in

[index.d.ts:7905](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7905)

___

### has

▸ **has**(`uri`): `boolean`

Check if this collection contains diagnostics for a
given resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | A resource identifier. |

#### Returns

`boolean`

`true` if this collection has diagnostic for the given resource.

#### Defined in

[index.d.ts:7914](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7914)

___

### set

▸ **set**(`uri`, `diagnostics`): `void`

Assign diagnostics for given resource. Will replace
existing diagnostics for that resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | A resource identifier. |
| `diagnostics` | `undefined` \| [`Diagnostic`](../classes/cloudide_plugin_.Diagnostic.md)[] | Array of diagnostics or `undefined` |

#### Returns

`void`

#### Defined in

[index.d.ts:7862](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7862)

▸ **set**(`entries`): `void`

Replace all entries in this collection for given uris.

Diagnostics of multiple tuples of the same uri will be merged, e.g
`[[file1, [d1]], [file1, [d2]]]` is equivalent to `[[file1, [d1, d2]]]`.
If a diagnostics item is `undefined` as in `[file1, undefined]`
all previous but not subsequent diagnostics are removed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `entries` | `undefined` \| [[`Uri`](../classes/cloudide_plugin_.Uri.md), `undefined` \| [`Diagnostic`](../classes/cloudide_plugin_.Diagnostic.md)[]][] | An array of tuples, like `[[file1, [d1, d2]], [file2, [d3, d4, d5]]]`, or `undefined`. |

#### Returns

`void`

#### Defined in

[index.d.ts:7874](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7874)
