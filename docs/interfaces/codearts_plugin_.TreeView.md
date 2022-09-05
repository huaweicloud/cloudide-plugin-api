[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TreeView

# Interface: TreeView<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).TreeView

Represents a Tree view

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

An optional human-readable description which is rendered less prominently in the title of the view.
Setting the title description to null, undefined, or empty string will remove the description from the view.

#### Defined in

[index.d.ts:10316](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10316)

___

### message

• `Optional` **message**: `string`

An optional human-readable message that will be rendered in the view.
Setting the message to null, undefined, or empty string will remove the message from the view.

#### Defined in

[index.d.ts:10304](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10304)

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewSelectionChangeEvent`](codearts_plugin_.TreeViewSelectionChangeEvent.md)<`T`\>\>

Event that is fired when the [selection](codearts_plugin_.TreeView.md#selection) has changed

#### Defined in

[index.d.ts:10288](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10288)

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewVisibilityChangeEvent`](codearts_plugin_.TreeViewVisibilityChangeEvent.md)\>

Event that is fired when [visibility](codearts_plugin_.TreeView.md#visible) has changed

#### Defined in

[index.d.ts:10298](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10298)

___

### onDidCollapseElement

• `Readonly` **onDidCollapseElement**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewExpansionEvent`](codearts_plugin_.TreeViewExpansionEvent.md)<`T`\>\>

Event that is fired when an element is collapsed

#### Defined in

[index.d.ts:10278](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10278)

___

### onDidExpandElement

• `Readonly` **onDidExpandElement**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewExpansionEvent`](codearts_plugin_.TreeViewExpansionEvent.md)<`T`\>\>

Event that is fired when an element is expanded

#### Defined in

[index.d.ts:10273](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10273)

___

### selection

• `Readonly` **selection**: readonly `T`[]

Currently selected elements.

#### Defined in

[index.d.ts:10283](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10283)

___

### title

• `Optional` **title**: `string`

The tree view title is initially taken from the extension package.json
Changes to the title property will be properly reflected in the UI in the title of the view.

#### Defined in

[index.d.ts:10310](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10310)

___

### visible

• `Readonly` **visible**: `boolean`

`true` if the [tree view](codearts_plugin_.TreeView.md) is visible otherwise `false`.

#### Defined in

[index.d.ts:10293](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10293)

## Methods

### dispose

▸ **dispose**(): `any`

Dispose this object.

#### Returns

`any`

#### Inherited from

[Disposable](../classes/codearts_plugin_.Disposable.md).[dispose](../classes/codearts_plugin_.Disposable.md#dispose)

#### Defined in

[index.d.ts:1580](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1580)

___

### reveal

▸ **reveal**(`element`, `options?`): [`Thenable`](Thenable.md)<`void`\>

Reveals the given element in the tree view.
If the tree view is not visible then the tree view is shown and element is revealed.

By default revealed element is selected.
In order to not to select, set the option `select` to `false`.
In order to focus, set the option `focus` to `true`.
In order to expand the revealed element, set the option `expand` to `true`. To expand recursively set `expand` to the number of levels to expand.
**NOTE:** You can expand only to 3 levels maximum.

**NOTE:** The [TreeDataProvider](codearts_plugin_.TreeDataProvider.md) that the `TreeView` [is registered with](../modules/codearts_plugin_.window.md#createtreeview) with must implement [getParent](codearts_plugin_.TreeDataProvider.md#getparent) method to access this API.

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

[index.d.ts:10330](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10330)
