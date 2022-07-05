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

[index.d.ts:8538](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L8538)

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:8567](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L8567)

___

### onDidDispose

• `Readonly` **onDidDispose**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:8548](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L8548)

___

### title

• `Optional` **title**: `string`

#### Defined in

[index.d.ts:8533](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L8533)

___

### viewType

• `Readonly` **viewType**: `string`

#### Defined in

[index.d.ts:8521](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L8521)

___

### visible

• `Readonly` **visible**: `boolean`

#### Defined in

[index.d.ts:8555](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L8555)

___

### webview

• `Readonly` **webview**: [`Webview`](codearts_plugin_.Webview.md)

#### Defined in

[index.d.ts:8526](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L8526)

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

[index.d.ts:8576](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L8576)
