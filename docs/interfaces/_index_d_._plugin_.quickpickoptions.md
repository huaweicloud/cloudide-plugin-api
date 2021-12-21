**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / QuickPickOptions

# Interface: QuickPickOptions

Options to configure the behavior of the quick pick UI.

## Hierarchy

* **QuickPickOptions**

## Index

### Properties

* [canPickMany](_index_d_._plugin_.quickpickoptions.md#canpickmany)
* [ignoreFocusOut](_index_d_._plugin_.quickpickoptions.md#ignorefocusout)
* [matchOnDescription](_index_d_._plugin_.quickpickoptions.md#matchondescription)
* [matchOnDetail](_index_d_._plugin_.quickpickoptions.md#matchondetail)
* [placeHolder](_index_d_._plugin_.quickpickoptions.md#placeholder)

### Methods

* [onDidSelectItem](_index_d_._plugin_.quickpickoptions.md#ondidselectitem)

## Properties

### canPickMany

• `Optional` **canPickMany**: boolean

*Defined in [index.d.ts:1809](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1809)*

An optional flag to make the picker accept multiple selections, if true the result is an array of picks.

___

### ignoreFocusOut

• `Optional` **ignoreFocusOut**: boolean

*Defined in [index.d.ts:1804](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1804)*

Set to `true` to keep the picker open when focus moves to another part of the editor or to another window.

___

### matchOnDescription

• `Optional` **matchOnDescription**: boolean

*Defined in [index.d.ts:1789](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1789)*

An optional flag to include the description when filtering the picks.

___

### matchOnDetail

• `Optional` **matchOnDetail**: boolean

*Defined in [index.d.ts:1794](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1794)*

An optional flag to include the detail when filtering the picks.

___

### placeHolder

• `Optional` **placeHolder**: string

*Defined in [index.d.ts:1799](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1799)*

An optional string to show as placeholder in the input box to guide the user what to pick on.

## Methods

### onDidSelectItem

▸ `Optional`**onDidSelectItem**(`item`: [QuickPickItem](_index_d_._plugin_.quickpickitem.md) \| string): any

*Defined in [index.d.ts:1814](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1814)*

An optional function that is invoked whenever an item is selected.

#### Parameters:

Name | Type |
------ | ------ |
`item` | [QuickPickItem](_index_d_._plugin_.quickpickitem.md) \| string |

**Returns:** any
