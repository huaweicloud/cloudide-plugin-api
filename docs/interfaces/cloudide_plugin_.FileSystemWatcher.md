[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FileSystemWatcher

# Interface: FileSystemWatcher

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FileSystemWatcher

A file system watcher notifies about changes to files and folders
on disk.

To get an instance of a `FileSystemWatcher` use
[createFileSystemWatcher](#workspace.createFileSystemWatcher).

## Hierarchy

- [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

  ↳ **`FileSystemWatcher`**

## Table of contents

### Properties

- [ignoreChangeEvents](cloudide_plugin_.FileSystemWatcher.md#ignorechangeevents)
- [ignoreCreateEvents](cloudide_plugin_.FileSystemWatcher.md#ignorecreateevents)
- [ignoreDeleteEvents](cloudide_plugin_.FileSystemWatcher.md#ignoredeleteevents)
- [onDidChange](cloudide_plugin_.FileSystemWatcher.md#ondidchange)
- [onDidCreate](cloudide_plugin_.FileSystemWatcher.md#ondidcreate)
- [onDidDelete](cloudide_plugin_.FileSystemWatcher.md#ondiddelete)

### Methods

- [dispose](cloudide_plugin_.FileSystemWatcher.md#dispose)

## Properties

### ignoreChangeEvents

• **ignoreChangeEvents**: `boolean`

true if this file system watcher has been created such that
it ignores change file system events.

#### Defined in

[index.d.ts:2069](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2069)

___

### ignoreCreateEvents

• **ignoreCreateEvents**: `boolean`

true if this file system watcher has been created such that
it ignores creation file system events.

#### Defined in

[index.d.ts:2063](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2063)

___

### ignoreDeleteEvents

• **ignoreDeleteEvents**: `boolean`

true if this file system watcher has been created such that
it ignores delete file system events.

#### Defined in

[index.d.ts:2075](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2075)

___

### onDidChange

• **onDidChange**: [`Event`](cloudide_plugin_.Event.md)<[`Uri`](../classes/cloudide_plugin_.Uri.md)\>

An event which fires on file/folder change.

#### Defined in

[index.d.ts:2085](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2085)

___

### onDidCreate

• **onDidCreate**: [`Event`](cloudide_plugin_.Event.md)<[`Uri`](../classes/cloudide_plugin_.Uri.md)\>

An event which fires on file/folder creation.

#### Defined in

[index.d.ts:2080](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2080)

___

### onDidDelete

• **onDidDelete**: [`Event`](cloudide_plugin_.Event.md)<[`Uri`](../classes/cloudide_plugin_.Uri.md)\>

An event which fires on file/folder deletion.

#### Defined in

[index.d.ts:2090](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2090)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this object.

#### Returns

`void`

#### Inherited from

[Disposable](../classes/cloudide_plugin_.Disposable.md).[dispose](../classes/cloudide_plugin_.Disposable.md#dispose)

#### Defined in

[index.d.ts:27](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L27)
