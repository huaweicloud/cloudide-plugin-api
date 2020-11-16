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

*Defined in [index.d.ts:1672](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1672)*

An optional flag to make the picker accept multiple selections, if true the result is an array of picks.

___

### ignoreFocusOut

• `Optional` **ignoreFocusOut**: boolean

*Defined in [index.d.ts:1667](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1667)*

Set to `true` to keep the picker open when focus moves to another part of the editor or to another window.

___

### matchOnDescription

• `Optional` **matchOnDescription**: boolean

*Defined in [index.d.ts:1652](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1652)*

An optional flag to include the description when filtering the picks.

___

### matchOnDetail

• `Optional` **matchOnDetail**: boolean

*Defined in [index.d.ts:1657](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1657)*

An optional flag to include the detail when filtering the picks.

___

### placeHolder

• `Optional` **placeHolder**: string

*Defined in [index.d.ts:1662](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1662)*

An optional string to show as placeholder in the input box to guide the user what to pick on.

## Methods

### onDidSelectItem

▸ `Optional`**onDidSelectItem**(`item`: [QuickPickItem](_index_d_._plugin_.quickpickitem.md) \| string): any

*Defined in [index.d.ts:1677](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1677)*

An optional function that is invoked whenever an item is selected.

#### Parameters:

Name | Type |
------ | ------ |
`item` | [QuickPickItem](_index_d_._plugin_.quickpickitem.md) \| string |

**Returns:** any
