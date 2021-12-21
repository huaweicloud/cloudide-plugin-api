**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TreeView

# Interface: TreeView\<T>

Represents a Tree view

## Type parameters

Name |
------ |
`T` |

## Hierarchy

* [Disposable](../classes/_index_d_._plugin_.disposable.md)

  ↳ **TreeView**

## Index

### Constructors

* [constructor](_index_d_._plugin_.treeview.md#constructor)

### Properties

* [description](_index_d_._plugin_.treeview.md#description)
* [message](_index_d_._plugin_.treeview.md#message)
* [onDidChangeSelection](_index_d_._plugin_.treeview.md#ondidchangeselection)
* [onDidChangeVisibility](_index_d_._plugin_.treeview.md#ondidchangevisibility)
* [onDidCollapseElement](_index_d_._plugin_.treeview.md#ondidcollapseelement)
* [onDidExpandElement](_index_d_._plugin_.treeview.md#ondidexpandelement)
* [selection](_index_d_._plugin_.treeview.md#selection)
* [title](_index_d_._plugin_.treeview.md#title)
* [visible](_index_d_._plugin_.treeview.md#visible)

### Methods

* [dispose](_index_d_._plugin_.treeview.md#dispose)
* [reveal](_index_d_._plugin_.treeview.md#reveal)
* [from](_index_d_._plugin_.treeview.md#from)

## Constructors

### constructor

\+ **new TreeView**(`callOnDispose`: Function): [TreeView](_index_d_._plugin_.treeview.md)

*Inherited from [Disposable](../classes/_index_d_._plugin_.disposable.md).[constructor](../classes/_index_d_._plugin_.disposable.md#constructor)*

*Defined in [index.d.ts:1601](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1601)*

Creates a new Disposable calling the provided function
on dispose.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`callOnDispose` | Function | Function that disposes something.  |

**Returns:** [TreeView](_index_d_._plugin_.treeview.md)

## Properties

### description

• `Optional` **description**: string

*Defined in [index.d.ts:9093](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9093)*

An optional human-readable description which is rendered less prominently in the title of the view.
Setting the title description to null, undefined, or empty string will remove the description from the view.

___

### message

• `Optional` **message**: string

*Defined in [index.d.ts:9081](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9081)*

An optional human-readable message that will be rendered in the view.
Setting the message to null, undefined, or empty string will remove the message from the view.

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [Event](_index_d_._plugin_.event.md)\<[TreeViewSelectionChangeEvent](_index_d_._plugin_.treeviewselectionchangeevent.md)\<T>>

*Defined in [index.d.ts:9065](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9065)*

Event that is fired when the [selection](#TreeView.selection) has changed

___

### onDidChangeVisibility

• `Readonly` **onDidChangeVisibility**: [Event](_index_d_._plugin_.event.md)\<[TreeViewVisibilityChangeEvent](_index_d_._plugin_.treeviewvisibilitychangeevent.md)>

*Defined in [index.d.ts:9075](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9075)*

Event that is fired when [visibility](#TreeView.visible) has changed

___

### onDidCollapseElement

• `Readonly` **onDidCollapseElement**: [Event](_index_d_._plugin_.event.md)\<[TreeViewExpansionEvent](_index_d_._plugin_.treeviewexpansionevent.md)\<T>>

*Defined in [index.d.ts:9055](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9055)*

Event that is fired when an element is collapsed

___

### onDidExpandElement

• `Readonly` **onDidExpandElement**: [Event](_index_d_._plugin_.event.md)\<[TreeViewExpansionEvent](_index_d_._plugin_.treeviewexpansionevent.md)\<T>>

*Defined in [index.d.ts:9050](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9050)*

Event that is fired when an element is expanded

___

### selection

• `Readonly` **selection**: T[]

*Defined in [index.d.ts:9060](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9060)*

Currently selected elements.

___

### title

• `Optional` **title**: string

*Defined in [index.d.ts:9087](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9087)*

The tree view title is initially taken from the extension package.json
Changes to the title property will be properly reflected in the UI in the title of the view.

___

### visible

• `Readonly` **visible**: boolean

*Defined in [index.d.ts:9070](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9070)*

`true` if the [tree view](#TreeView) is visible otherwise `false`.

## Methods

### dispose

▸ **dispose**(): any

*Inherited from [Disposable](../classes/_index_d_._plugin_.disposable.md).[dispose](../classes/_index_d_._plugin_.disposable.md#dispose)*

*Defined in [index.d.ts:1613](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1613)*

Dispose this object.

**Returns:** any

___

### reveal

▸ **reveal**(`element`: T, `options?`: { expand?: boolean \| number ; focus?: boolean ; select?: boolean  }): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:9107](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9107)*

Reveals the given element in the tree view.
If the tree view is not visible then the tree view is shown and element is revealed.

By default revealed element is selected.
In order to not to select, set the option `select` to `false`.
In order to focus, set the option `focus` to `true`.
In order to expand the revealed element, set the option `expand` to `true`. To expand recursively set `expand` to the number of levels to expand.
**NOTE:** You can expand only to 3 levels maximum.

**NOTE:** The [TreeDataProvider](#TreeDataProvider) that the `TreeView` [is registered with](#window.createTreeView) with must implement [getParent](#TreeDataProvider.getParent) method to access this API.

#### Parameters:

Name | Type |
------ | ------ |
`element` | T |
`options?` | { expand?: boolean \| number ; focus?: boolean ; select?: boolean  } |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

___

### from

▸ `Static`**from**(...`disposableLikes`: { dispose: () => any  }[]): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Inherited from [Disposable](../classes/_index_d_._plugin_.disposable.md).[from](../classes/_index_d_._plugin_.disposable.md#from)*

*Defined in [index.d.ts:1601](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1601)*

Combine many disposable-likes into one. Use this method
when having objects with a dispose function which are not
instances of Disposable.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`...disposableLikes` | { dispose: () => any  }[] | Objects that have at least a `dispose`-function member. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

Returns a new disposable which, upon dispose, will
dispose all provided disposables.
