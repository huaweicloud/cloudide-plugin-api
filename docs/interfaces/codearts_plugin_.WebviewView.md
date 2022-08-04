[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WebviewView

# Interface: WebviewView

["@codearts/plugin"](../modules/_codearts_plugin_.md).WebviewView

## Table of contents

### Properties

- [description](codearts_plugin_.WebviewView.md#description)
- [onDidChangeVisibility](codearts_plugin_.WebviewView.md#ondidchangevisibility)
- [onDidDispose](codearts_plugin_.WebviewView.md#ondiddispose)
- [title](codearts_plugin_.WebviewView.md#title)
- [viewType](codearts_plugin_.WebviewView.md#viewtype)
- [visible](codearts_plugin_.WebviewView.md#visible)
- [webview](codearts_plugin_.WebviewView.md#webview)

### Methods

- [show](codearts_plugin_.WebviewView.md#show)

## Properties

### description

• `Optional` **description**: `string`

#### Defined in

[index.d.ts:8556](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8556)

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:8585](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8585)

___

### onDidDispose

• `Readonly` **onDidDispose**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:8566](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8566)

___

### title

• `Optional` **title**: `string`

#### Defined in

[index.d.ts:8551](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8551)

___

### viewType

• `Readonly` **viewType**: `string`

#### Defined in

[index.d.ts:8539](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8539)

___

### visible

• `Readonly` **visible**: `boolean`

#### Defined in

[index.d.ts:8573](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8573)

___

### webview

• `Readonly` **webview**: [`Webview`](codearts_plugin_.Webview.md)

#### Defined in

[index.d.ts:8544](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8544)

## Methods

### show

▸ **show**(`preserveFocus?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `preserveFocus?` | `boolean` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:8594](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L8594)
