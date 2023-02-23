[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TreeView

# Interface: TreeView<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TreeView

Represents a Tree view

## Type parameters

| Name |
| :------ |
| `T` |

## Hierarchy

- [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

  ↳ **`TreeView`**

## Table of contents

### Properties

- [description](cloudide_plugin_.TreeView.md#description)
- [message](cloudide_plugin_.TreeView.md#message)
- [onDidChangeSelection](cloudide_plugin_.TreeView.md#ondidchangeselection)
- [onDidChangeVisibility](cloudide_plugin_.TreeView.md#ondidchangevisibility)
- [onDidCollapseElement](cloudide_plugin_.TreeView.md#ondidcollapseelement)
- [onDidExpandElement](cloudide_plugin_.TreeView.md#ondidexpandelement)
- [selection](cloudide_plugin_.TreeView.md#selection)
- [title](cloudide_plugin_.TreeView.md#title)
- [visible](cloudide_plugin_.TreeView.md#visible)

### Methods

- [dispose](cloudide_plugin_.TreeView.md#dispose)
- [reveal](cloudide_plugin_.TreeView.md#reveal)

## Properties

### description

• `Optional` **description**: `string`

An optional human-readable subheading that will be rendered next to the main title.
Setting the description to null, undefined, or empty string will remove the message from the view.

#### Defined in

[index.d.ts:5254](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5254)

___

### message

• `Optional` **message**: `string`

An optional human-readable message that will be rendered in the view.
Setting the message to null, undefined, or empty string will remove the message from the view.

#### Defined in

[index.d.ts:5242](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5242)

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [`Event`](cloudide_plugin_.Event.md)<[`TreeViewSelectionChangeEvent`](cloudide_plugin_.TreeViewSelectionChangeEvent.md)<`T`\>\>

Event that is fired when the [selection](#TreeView.selection) has changed

#### Defined in

[index.d.ts:5226](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5226)

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [`Event`](cloudide_plugin_.Event.md)<[`TreeViewVisibilityChangeEvent`](cloudide_plugin_.TreeViewVisibilityChangeEvent.md)\>

Event that is fired when [visibility](#TreeView.visible) has changed

#### Defined in

[index.d.ts:5236](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5236)

___

### onDidCollapseElement

• `Readonly` **onDidCollapseElement**: [`Event`](cloudide_plugin_.Event.md)<[`TreeViewExpansionEvent`](cloudide_plugin_.TreeViewExpansionEvent.md)<`T`\>\>

Event that is fired when an element is collapsed

#### Defined in

[index.d.ts:5216](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5216)

___

### onDidExpandElement

• `Readonly` **onDidExpandElement**: [`Event`](cloudide_plugin_.Event.md)<[`TreeViewExpansionEvent`](cloudide_plugin_.TreeViewExpansionEvent.md)<`T`\>\>

Event that is fired when an element is expanded

#### Defined in

[index.d.ts:5211](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5211)

___

### selection

• `Readonly` **selection**: readonly `T`[]

Currently selected elements.

#### Defined in

[index.d.ts:5221](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5221)

___

### title

• `Optional` **title**: `string`

The tree view title is initially taken from the extension package.json
Changes to the title property will be properly reflected in the UI in the title of the view.

#### Defined in

[index.d.ts:5248](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5248)

___

### visible

• `Readonly` **visible**: `boolean`

`true` if the [tree view](#TreeView) is visible otherwise `false`.

#### Defined in

[index.d.ts:5231](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5231)

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

___

### reveal

▸ **reveal**(`element`, `options?`): `PromiseLike`<`void`\>

Reveal an element. By default revealed element is selected.

In order to not to select, set the option `select` to `false`.

**NOTE:** [TreeDataProvider](#TreeDataProvider) is required to implement [getParent](#TreeDataProvider.getParent) method to access this API.

#### Parameters

| Name | Type |
| :------ | :------ |
| `element` | `T` |
| `options?` | `Object` |
| `options.expand?` | `number` \| `boolean` |
| `options.focus?` | `boolean` |
| `options.select?` | `boolean` |

#### Returns

`PromiseLike`<`void`\>

#### Defined in

[index.d.ts:5263](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5263)
