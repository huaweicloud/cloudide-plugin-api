[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileSystemWatcher

# Interface: FileSystemWatcher

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileSystemWatcher

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

• **ignoreChangeEvents**: `boolean`

#### Defined in

[index.d.ts:1655](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L1655)

___

### ignoreCreateEvents

• **ignoreCreateEvents**: `boolean`

#### Defined in

[index.d.ts:1649](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L1649)

___

### ignoreDeleteEvents

• **ignoreDeleteEvents**: `boolean`

#### Defined in

[index.d.ts:1661](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L1661)

___

### onDidChange

• **onDidChange**: [`Event`](codearts_plugin_.Event.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

#### Defined in

[index.d.ts:1671](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L1671)

___

### onDidCreate

• **onDidCreate**: [`Event`](codearts_plugin_.Event.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

#### Defined in

[index.d.ts:1666](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L1666)

___

### onDidDelete

• **onDidDelete**: [`Event`](codearts_plugin_.Event.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

#### Defined in

[index.d.ts:1676](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L1676)

## Methods

### dispose

▸ **dispose**(): `any`

#### Returns

`any`

#### Inherited from

[Disposable](../classes/codearts_plugin_.Disposable.md).[dispose](../classes/codearts_plugin_.Disposable.md#dispose)

#### Defined in

[index.d.ts:1580](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L1580)
