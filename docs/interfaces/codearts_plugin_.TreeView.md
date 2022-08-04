[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TreeView

# Interface: TreeView<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).TreeView

## Type parameters

| Name |
| :------ |
| `T` |

## Hierarchy

- [`Disposable`](../classes/codearts_plugin_.Disposable.md)

  ↳ **`TreeView`**

## Table of contents

### Properties

- [description](codearts_plugin_.TreeView.md#description)
- [message](codearts_plugin_.TreeView.md#message)
- [onDidChangeSelection](codearts_plugin_.TreeView.md#ondidchangeselection)
- [onDidChangeVisibility](codearts_plugin_.TreeView.md#ondidchangevisibility)
- [onDidCollapseElement](codearts_plugin_.TreeView.md#ondidcollapseelement)
- [onDidExpandElement](codearts_plugin_.TreeView.md#ondidexpandelement)
- [selection](codearts_plugin_.TreeView.md#selection)
- [title](codearts_plugin_.TreeView.md#title)
- [visible](codearts_plugin_.TreeView.md#visible)

### Methods

- [dispose](codearts_plugin_.TreeView.md#dispose)
- [reveal](codearts_plugin_.TreeView.md#reveal)

## Properties

### description

• `Optional` **description**: `string`

#### Defined in

[index.d.ts:10254](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10254)

___

### message

• `Optional` **message**: `string`

#### Defined in

[index.d.ts:10242](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10242)

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewSelectionChangeEvent`](codearts_plugin_.TreeViewSelectionChangeEvent.md)<`T`\>\>

#### Defined in

[index.d.ts:10226](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10226)

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewVisibilityChangeEvent`](codearts_plugin_.TreeViewVisibilityChangeEvent.md)\>

#### Defined in

[index.d.ts:10236](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10236)

___

### onDidCollapseElement

• `Readonly` **onDidCollapseElement**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewExpansionEvent`](codearts_plugin_.TreeViewExpansionEvent.md)<`T`\>\>

#### Defined in

[index.d.ts:10216](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10216)

___

### onDidExpandElement

• `Readonly` **onDidExpandElement**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewExpansionEvent`](codearts_plugin_.TreeViewExpansionEvent.md)<`T`\>\>

#### Defined in

[index.d.ts:10211](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10211)

___

### selection

• `Readonly` **selection**: readonly `T`[]

#### Defined in

[index.d.ts:10221](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10221)

___

### title

• `Optional` **title**: `string`

#### Defined in

[index.d.ts:10248](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10248)

___

### visible

• `Readonly` **visible**: `boolean`

#### Defined in

[index.d.ts:10231](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10231)

## Methods

### dispose

▸ **dispose**(): `any`

#### Returns

`any`

#### Inherited from

[Disposable](../classes/codearts_plugin_.Disposable.md).[dispose](../classes/codearts_plugin_.Disposable.md#dispose)

#### Defined in

[index.d.ts:1580](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L1580)

___

### reveal

▸ **reveal**(`element`, `options?`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `element` | `T` |
| `options?` | `Object` |
| `options.expand?` | `number` \| `boolean` |
| `options.focus?` | `boolean` |
| `options.select?` | `boolean` |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:10268](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10268)
