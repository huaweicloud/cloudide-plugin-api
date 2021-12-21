**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Disposable

# Class: Disposable

Represents a type which can release resources, such
as event listening or a timer.

## Hierarchy

* **Disposable**

  ↳ [FileSystemWatcher](../interfaces/_index_d_._plugin_.filesystemwatcher.md)

  ↳ [TreeView](../interfaces/_index_d_._plugin_.treeview.md)

  ↳ [DebugAdapter](../interfaces/_index_d_._plugin_.debugadapter.md)

## Index

### Constructors

* [constructor](_index_d_._plugin_.disposable.md#constructor)

### Methods

* [dispose](_index_d_._plugin_.disposable.md#dispose)
* [from](_index_d_._plugin_.disposable.md#from)

## Constructors

### constructor

\+ **new Disposable**(`callOnDispose`: Function): [Disposable](_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:1601](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1601)*

Creates a new Disposable calling the provided function
on dispose.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`callOnDispose` | Function | Function that disposes something.  |

**Returns:** [Disposable](_index_d_._plugin_.disposable.md)

## Methods

### dispose

▸ **dispose**(): any

*Defined in [index.d.ts:1613](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1613)*

Dispose this object.

**Returns:** any

___

### from

▸ `Static`**from**(...`disposableLikes`: { dispose: () => any  }[]): [Disposable](_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:1601](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1601)*

Combine many disposable-likes into one. Use this method
when having objects with a dispose function which are not
instances of Disposable.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`...disposableLikes` | { dispose: () => any  }[] | Objects that have at least a `dispose`-function member. |

**Returns:** [Disposable](_index_d_._plugin_.disposable.md)

Returns a new disposable which, upon dispose, will
dispose all provided disposables.
