**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DiagnosticCollection

# Interface: DiagnosticCollection

A diagnostics collection is a container that manages a set of
[diagnostics](#Diagnostic). Diagnostics are always scopes to a
diagnostics collection and a resource.

To get an instance of a `DiagnosticCollection` use
[createDiagnosticCollection](#languages.createDiagnosticCollection).

## Hierarchy

* **DiagnosticCollection**

## Index

### Properties

* [name](_index_d_._plugin_.diagnosticcollection.md#name)

### Methods

* [clear](_index_d_._plugin_.diagnosticcollection.md#clear)
* [delete](_index_d_._plugin_.diagnosticcollection.md#delete)
* [dispose](_index_d_._plugin_.diagnosticcollection.md#dispose)
* [forEach](_index_d_._plugin_.diagnosticcollection.md#foreach)
* [get](_index_d_._plugin_.diagnosticcollection.md#get)
* [has](_index_d_._plugin_.diagnosticcollection.md#has)
* [set](_index_d_._plugin_.diagnosticcollection.md#set)

## Properties

### name

• `Readonly` **name**: string

*Defined in [index.d.ts:5303](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5303)*

The name of this diagnostic collection, for instance `typescript`. Every diagnostic
from this collection will be associated with this name. Also, the task framework uses this
name when defining [problem matchers](https://code.visualstudio.com/docs/editor/tasks#_defining-a-problem-matcher).

## Methods

### clear

▸ **clear**(): void

*Defined in [index.d.ts:5338](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5338)*

Remove all diagnostics from this collection. The same
as calling `#set(undefined)`;

**Returns:** void

___

### delete

▸ **delete**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): void

*Defined in [index.d.ts:5332](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5332)*

Remove all diagnostics from this collection that belong
to the provided `uri`. The same as `#set(uri, undefined)`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | A resource identifier.  |

**Returns:** void

___

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:5370](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5370)*

Dispose and free associated resources. Calls
[clear](#DiagnosticCollection.clear).

**Returns:** void

___

### forEach

▸ **forEach**(`callback`: (uri: [Uri](../classes/_index_d_._plugin_.uri.md), diagnostics: ReadonlyArray\<[Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)>, collection: [DiagnosticCollection](_index_d_._plugin_.diagnosticcollection.md)) => any, `thisArg?`: any): void

*Defined in [index.d.ts:5346](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5346)*

Iterate over each entry in this collection.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`callback` | (uri: [Uri](../classes/_index_d_._plugin_.uri.md), diagnostics: ReadonlyArray\<[Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)>, collection: [DiagnosticCollection](_index_d_._plugin_.diagnosticcollection.md)) => any | Function to execute for each entry. |
`thisArg?` | any | The `this` context used when invoking the handler function.  |

**Returns:** void

___

### get

▸ **get**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): ReadonlyArray\<[Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)> \| undefined

*Defined in [index.d.ts:5355](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5355)*

Get the diagnostics for a given resource. *Note* that you cannot
modify the diagnostics-array returned from this call.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | A resource identifier. |

**Returns:** ReadonlyArray\<[Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)> \| undefined

An immutable array of [diagnostics](#Diagnostic) or `undefined`.

___

### has

▸ **has**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): boolean

*Defined in [index.d.ts:5364](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5364)*

Check if this collection contains diagnostics for a
given resource.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | A resource identifier. |

**Returns:** boolean

`true` if this collection has diagnostic for the given resource.

___

### set

▸ **set**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `diagnostics`: ReadonlyArray\<[Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)> \| undefined): void

*Defined in [index.d.ts:5312](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5312)*

Assign diagnostics for given resource. Will replace
existing diagnostics for that resource.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | A resource identifier. |
`diagnostics` | ReadonlyArray\<[Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)> \| undefined | Array of diagnostics or `undefined`  |

**Returns:** void

▸ **set**(`entries`: ReadonlyArray\<[[Uri](../classes/_index_d_._plugin_.uri.md), ReadonlyArray\<[Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)> \| undefined]>): void

*Defined in [index.d.ts:5324](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5324)*

Replace diagnostics for multiple resources in this collection.

 _Note_ that multiple tuples of the same uri will be merged, e.g
`[[file1, [d1]], [file1, [d2]]]` is equivalent to `[[file1, [d1, d2]]]`.
If a diagnostics item is `undefined` as in `[file1, undefined]`
all previous but not subsequent diagnostics are removed.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`entries` | ReadonlyArray\<[[Uri](../classes/_index_d_._plugin_.uri.md), ReadonlyArray\<[Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)> \| undefined]> | An array of tuples, like `[[file1, [d1, d2]], [file2, [d3, d4, d5]]]`, or `undefined`.  |

**Returns:** void
