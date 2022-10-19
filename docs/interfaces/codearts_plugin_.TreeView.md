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

[index.d.ts:10469](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10469)

___

### message

• `Optional` **message**: `string`

An optional human-readable message that will be rendered in the view.
Setting the message to null, undefined, or empty string will remove the message from the view.

#### Defined in

[index.d.ts:10457](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10457)

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewSelectionChangeEvent`](codearts_plugin_.TreeViewSelectionChangeEvent.md)<`T`\>\>

Event that is fired when the [selection](codearts_plugin_.TreeView.md#selection) has changed

#### Defined in

[index.d.ts:10441](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10441)

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewVisibilityChangeEvent`](codearts_plugin_.TreeViewVisibilityChangeEvent.md)\>

Event that is fired when [visibility](codearts_plugin_.TreeView.md#visible) has changed

#### Defined in

[index.d.ts:10451](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10451)

___

### onDidCollapseElement

• `Readonly` **onDidCollapseElement**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewExpansionEvent`](codearts_plugin_.TreeViewExpansionEvent.md)<`T`\>\>

Event that is fired when an element is collapsed

#### Defined in

[index.d.ts:10431](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10431)

___

### onDidExpandElement

• `Readonly` **onDidExpandElement**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewExpansionEvent`](codearts_plugin_.TreeViewExpansionEvent.md)<`T`\>\>

Event that is fired when an element is expanded

#### Defined in

[index.d.ts:10426](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10426)

___

### selection

• `Readonly` **selection**: readonly `T`[]

Currently selected elements.

#### Defined in

[index.d.ts:10436](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10436)

___

### title

• `Optional` **title**: `string`

The tree view title is initially taken from the extension package.json
Changes to the title property will be properly reflected in the UI in the title of the view.

#### Defined in

[index.d.ts:10463](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10463)

___

### visible

• `Readonly` **visible**: `boolean`

`true` if the [tree view](codearts_plugin_.TreeView.md) is visible otherwise `false`.

#### Defined in

[index.d.ts:10446](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10446)

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

[index.d.ts:10483](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10483)
