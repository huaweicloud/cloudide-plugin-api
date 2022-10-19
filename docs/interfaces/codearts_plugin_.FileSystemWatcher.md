[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileSystemWatcher

# Interface: FileSystemWatcher

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileSystemWatcher

A file system watcher notifies about changes to files and folders
on disk or from other [FileSystemProviders](codearts_plugin_.FileSystemProvider.md).

To get an instance of a `FileSystemWatcher` use
[createFileSystemWatcher](../modules/codearts_plugin_.workspace.md#createfilesystemwatcher).

## Hierarchy

- [`Disposable`](../classes/codearts_plugin_.Disposable.md)

  ↳ **`FileSystemWatcher`**

## Table of contents

### Properties

- [ignoreChangeEvents](codearts_plugin_.FileSystemWatcher.md#ignorechangeevents)
- [ignoreCreateEvents](codearts_plugin_.FileSystemWatcher.md#ignorecreateevents)
- [ignoreDeleteEvents](codearts_plugin_.FileSystemWatcher.md#ignoredeleteevents)
- [onDidChange](codearts_plugin_.FileSystemWatcher.md#ondidchange)
- [onDidCreate](codearts_plugin_.FileSystemWatcher.md#ondidcreate)
- [onDidDelete](codearts_plugin_.FileSystemWatcher.md#ondiddelete)

### Methods

- [dispose](codearts_plugin_.FileSystemWatcher.md#dispose)

## Properties

### ignoreChangeEvents

• `Readonly` **ignoreChangeEvents**: `boolean`

true if this file system watcher has been created such that
it ignores change file system events.

#### Defined in

[index.d.ts:1655](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1655)

___

### ignoreCreateEvents

• `Readonly` **ignoreCreateEvents**: `boolean`

true if this file system watcher has been created such that
it ignores creation file system events.

#### Defined in

[index.d.ts:1649](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1649)

___

### ignoreDeleteEvents

• `Readonly` **ignoreDeleteEvents**: `boolean`

true if this file system watcher has been created such that
it ignores delete file system events.

#### Defined in

[index.d.ts:1661](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1661)

___

### onDidChange

• `Readonly` **onDidChange**: [`Event`](codearts_plugin_.Event.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

An event which fires on file/folder change.

#### Defined in

[index.d.ts:1671](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1671)

___

### onDidCreate

• `Readonly` **onDidCreate**: [`Event`](codearts_plugin_.Event.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

An event which fires on file/folder creation.

#### Defined in

[index.d.ts:1666](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1666)

___

### onDidDelete

• `Readonly` **onDidDelete**: [`Event`](codearts_plugin_.Event.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

An event which fires on file/folder deletion.

#### Defined in

[index.d.ts:1676](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1676)

## Methods

### dispose

▸ **dispose**(): `any`

Dispose this object.

#### Returns

`any`

#### Inherited from

[Disposable](../classes/codearts_plugin_.Disposable.md).[dispose](../classes/codearts_plugin_.Disposable.md#dispose)

#### Defined in

[index.d.ts:1580](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1580)
