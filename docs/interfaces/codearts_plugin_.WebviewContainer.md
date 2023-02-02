[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WebviewContainer

# Interface: WebviewContainer

["@codearts/plugin"](../modules/_codearts_plugin_.md).WebviewContainer

A viewContainer that contains a webview.

## Table of contents

### Properties

- [onDidDispose](codearts_plugin_.WebviewContainer.md#ondiddispose)
- [viewType](codearts_plugin_.WebviewContainer.md#viewtype)
- [webview](codearts_plugin_.WebviewContainer.md#webview)

### Methods

- [dispose](codearts_plugin_.WebviewContainer.md#dispose)
- [reveal](codearts_plugin_.WebviewContainer.md#reveal)

## Properties

### onDidDispose

• `Readonly` **onDidDispose**: (`handlerDispose`: () => `void`) => `void`

#### Type declaration

▸ (`handlerDispose`): `void`

Fired when the container is disposed.

This may be because the user closed the container or because `.dispose()` was
called on it.

Trying to use the container after it has been disposed throws an exception.

##### Parameters

| Name | Type |
| :------ | :------ |
| `handlerDispose` | () => `void` |

##### Returns

`void`

#### Defined in

[index.d.ts:8553](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8553)

___

### viewType

• `Readonly` **viewType**: `string`

Identifies the type of the webview container.

#### Defined in

[index.d.ts:8533](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8533)

___

### webview

• **webview**: `any`

Webview of the container.

#### Defined in

[index.d.ts:8543](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8543)

## Methods

### dispose

▸ **dispose**(): `any`

Dispose of the container.

#### Returns

`any`

#### Defined in

[index.d.ts:8538](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8538)

___

### reveal

▸ **reveal**(`viewColumn?`, `preserveFocus?`): `void`

Show the webview container in a given column.

A webview container may only show in a single column at a time. If it is already showing, this
method moves it to a new column.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewColumn?` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) | View column to show the panel in. Shows in the current `viewColumn` if undefined. |
| `preserveFocus?` | `boolean` | When `true`, the webview will not take focus. |

#### Returns

`void`

#### Defined in

[index.d.ts:8564](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8564)
