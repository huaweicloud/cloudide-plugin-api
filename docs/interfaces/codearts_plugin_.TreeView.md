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
- [focusedElements](codearts_plugin_.TreeView.md#focusedelements)
- [message](codearts_plugin_.TreeView.md#message)
- [onDidChangeFocus](codearts_plugin_.TreeView.md#ondidchangefocus)
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
- [showEditBox](codearts_plugin_.TreeView.md#showeditbox)

## Properties

### description

• `Optional` **description**: `string`

An optional human-readable description which is rendered less prominently in the title of the view.
Setting the title description to null, undefined, or empty string will remove the description from the view.

#### Defined in

[index.d.ts:10725](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10725)

___

### focusedElements

• `Readonly` **focusedElements**: readonly `T`[]

Currently focused elements.

#### Defined in

[index.d.ts:10692](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10692)

___

### message

• `Optional` **message**: `string`

An optional human-readable message that will be rendered in the view.
Setting the message to null, undefined, or empty string will remove the message from the view.

#### Defined in

[index.d.ts:10713](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10713)

___

### onDidChangeFocus

• `Readonly` **onDidChangeFocus**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewFocusChangeEvent`](codearts_plugin_.TreeViewFocusChangeEvent.md)<`T`\>\>

Event that is fired when the [focused elements](codearts_plugin_.TreeView.md#focusedelements) have changed

#### Defined in

[index.d.ts:10697](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10697)

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewSelectionChangeEvent`](codearts_plugin_.TreeViewSelectionChangeEvent.md)<`T`\>\>

Event that is fired when the [selection](codearts_plugin_.TreeView.md#selection) has changed

#### Defined in

[index.d.ts:10687](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10687)

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewVisibilityChangeEvent`](codearts_plugin_.TreeViewVisibilityChangeEvent.md)\>

Event that is fired when [visibility](codearts_plugin_.TreeView.md#visible) has changed

#### Defined in

[index.d.ts:10707](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10707)

___

### onDidCollapseElement

• `Readonly` **onDidCollapseElement**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewExpansionEvent`](codearts_plugin_.TreeViewExpansionEvent.md)<`T`\>\>

Event that is fired when an element is collapsed

#### Defined in

[index.d.ts:10677](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10677)

___

### onDidExpandElement

• `Readonly` **onDidExpandElement**: [`Event`](codearts_plugin_.Event.md)<[`TreeViewExpansionEvent`](codearts_plugin_.TreeViewExpansionEvent.md)<`T`\>\>

Event that is fired when an element is expanded

#### Defined in

[index.d.ts:10672](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10672)

___

### selection

• `Readonly` **selection**: readonly `T`[]

Currently selected elements.

#### Defined in

[index.d.ts:10682](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10682)

___

### title

• `Optional` **title**: `string`

The tree view title is initially taken from the extension package.json
Changes to the title property will be properly reflected in the UI in the title of the view.

#### Defined in

[index.d.ts:10719](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10719)

___

### visible

• `Readonly` **visible**: `boolean`

`true` if the [tree view](codearts_plugin_.TreeView.md) is visible otherwise `false`.

#### Defined in

[index.d.ts:10702](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10702)

## Methods

### dispose

▸ **dispose**(): `any`

Dispose this object.

#### Returns

`any`

#### Inherited from

[Disposable](../classes/codearts_plugin_.Disposable.md).[dispose](../classes/codearts_plugin_.Disposable.md#dispose)

#### Defined in

[index.d.ts:1580](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1580)

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

[index.d.ts:10739](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10739)

___

### showEditBox

▸ **showEditBox**(`element`, `options?`): [`Thenable`](Thenable.md)<`undefined` \| `string`\>

Opens an edit box on given element in the tree view.

The returned value will be `undefined` if the edit box was canceled (e.g. pressing ESC). Otherwise the
returned value will be the string typed by the user or an empty string if the user did not type
anything but dismissed the input box with OK.
When the input is out of focus, it will return undefined.
On the premise that the verification is passed, when the enter key is pressed or the focus is lost, the input value will be returned.
When the verification fails and the focus is out of focus, it will return undefined.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `T` | the element on which the edit box is shown |
| `options?` | [`TreeViewEditBoxOptions`](codearts_plugin_.TreeViewEditBoxOptions.md) | Configures the behavior of the edit box. |

#### Returns

[`Thenable`](Thenable.md)<`undefined` \| `string`\>

A promise that resolves to a string the user provided or to `undefined` in case of dismissal.

#### Defined in

[index.d.ts:10754](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10754)
