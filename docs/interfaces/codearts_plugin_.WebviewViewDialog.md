[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WebviewViewDialog

# Interface: WebviewViewDialog

["@codearts/plugin"](../modules/_codearts_plugin_.md).WebviewViewDialog

A dialog that contains a webview view.

## Hierarchy

- [`Disposable`](../classes/codearts_plugin_.Disposable.md)

  ↳ **`WebviewViewDialog`**

## Table of contents

### Properties

- [onDidDispose](codearts_plugin_.WebviewViewDialog.md#ondiddispose)

### Methods

- [dispose](codearts_plugin_.WebviewViewDialog.md#dispose)

## Properties

### onDidDispose

• `Readonly` **onDidDispose**: [`Event`](codearts_plugin_.Event.md)<`void`\>

Fired when the webviewview dialog is disposed.

This may be because the user closed the dialog or because `.dispose()` was
called on it.

#### Defined in

[index.d.ts:8467](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L8467)

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
