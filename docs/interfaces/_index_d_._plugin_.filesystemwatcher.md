**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileSystemWatcher

# Interface: FileSystemWatcher

A file system watcher notifies about changes to files and folders
on disk or from other [FileSystemProviders](#FileSystemProvider).

To get an instance of a `FileSystemWatcher` use
[createFileSystemWatcher](#workspace.createFileSystemWatcher).

## Hierarchy

* [Disposable](../classes/_index_d_._plugin_.disposable.md)

  ↳ **FileSystemWatcher**

## Index

### Constructors

* [constructor](_index_d_._plugin_.filesystemwatcher.md#constructor)

### Properties

* [ignoreChangeEvents](_index_d_._plugin_.filesystemwatcher.md#ignorechangeevents)
* [ignoreCreateEvents](_index_d_._plugin_.filesystemwatcher.md#ignorecreateevents)
* [ignoreDeleteEvents](_index_d_._plugin_.filesystemwatcher.md#ignoredeleteevents)
* [onDidChange](_index_d_._plugin_.filesystemwatcher.md#ondidchange)
* [onDidCreate](_index_d_._plugin_.filesystemwatcher.md#ondidcreate)
* [onDidDelete](_index_d_._plugin_.filesystemwatcher.md#ondiddelete)

### Methods

* [dispose](_index_d_._plugin_.filesystemwatcher.md#dispose)
* [from](_index_d_._plugin_.filesystemwatcher.md#from)

## Constructors

### constructor

\+ **new FileSystemWatcher**(`callOnDispose`: Function): [FileSystemWatcher](_index_d_._plugin_.filesystemwatcher.md)

*Inherited from [Disposable](../classes/_index_d_._plugin_.disposable.md).[constructor](../classes/_index_d_._plugin_.disposable.md#constructor)*

*Defined in [index.d.ts:1601](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1601)*

Creates a new Disposable calling the provided function
on dispose.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`callOnDispose` | Function | Function that disposes something.  |

**Returns:** [FileSystemWatcher](_index_d_._plugin_.filesystemwatcher.md)

## Properties

### ignoreChangeEvents

•  **ignoreChangeEvents**: boolean

*Defined in [index.d.ts:1687](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1687)*

true if this file system watcher has been created such that
it ignores change file system events.

___

### ignoreCreateEvents

•  **ignoreCreateEvents**: boolean

*Defined in [index.d.ts:1681](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1681)*

true if this file system watcher has been created such that
it ignores creation file system events.

___

### ignoreDeleteEvents

•  **ignoreDeleteEvents**: boolean

*Defined in [index.d.ts:1693](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1693)*

true if this file system watcher has been created such that
it ignores delete file system events.

___

### onDidChange

•  **onDidChange**: [Event](_index_d_._plugin_.event.md)\<[Uri](../classes/_index_d_._plugin_.uri.md)>

*Defined in [index.d.ts:1703](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1703)*

An event which fires on file/folder change.

___

### onDidCreate

•  **onDidCreate**: [Event](_index_d_._plugin_.event.md)\<[Uri](../classes/_index_d_._plugin_.uri.md)>

*Defined in [index.d.ts:1698](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1698)*

An event which fires on file/folder creation.

___

### onDidDelete

•  **onDidDelete**: [Event](_index_d_._plugin_.event.md)\<[Uri](../classes/_index_d_._plugin_.uri.md)>

*Defined in [index.d.ts:1708](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1708)*

An event which fires on file/folder deletion.

## Methods

### dispose

▸ **dispose**(): any

*Inherited from [Disposable](../classes/_index_d_._plugin_.disposable.md).[dispose](../classes/_index_d_._plugin_.disposable.md#dispose)*

*Defined in [index.d.ts:1613](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1613)*

Dispose this object.

**Returns:** any

___

### from

▸ `Static`**from**(...`disposableLikes`: { dispose: () => any  }[]): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Inherited from [Disposable](../classes/_index_d_._plugin_.disposable.md).[from](../classes/_index_d_._plugin_.disposable.md#from)*

*Defined in [index.d.ts:1601](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1601)*

Combine many disposable-likes into one. Use this method
when having objects with a dispose function which are not
instances of Disposable.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`...disposableLikes` | { dispose: () => any  }[] | Objects that have at least a `dispose`-function member. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

Returns a new disposable which, upon dispose, will
dispose all provided disposables.
