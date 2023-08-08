[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / QuickPickOptions

# Interface: QuickPickOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).QuickPickOptions

Options to configure the behavior of the quick pick UI.

## Table of contents

### Properties

- [canPickMany](codearts_plugin_.QuickPickOptions.md#canpickmany)
- [ignoreFocusOut](codearts_plugin_.QuickPickOptions.md#ignorefocusout)
- [matchOnDescription](codearts_plugin_.QuickPickOptions.md#matchondescription)
- [matchOnDetail](codearts_plugin_.QuickPickOptions.md#matchondetail)
- [placeHolder](codearts_plugin_.QuickPickOptions.md#placeholder)
- [title](codearts_plugin_.QuickPickOptions.md#title)

### Methods

- [onDidSelectItem](codearts_plugin_.QuickPickOptions.md#ondidselectitem)

## Properties

### canPickMany

• `Optional` **canPickMany**: `boolean`

An optional flag to make the picker accept multiple selections, if true the result is an array of picks.

#### Defined in

[index.d.ts:1825](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1825)

___

### ignoreFocusOut

• `Optional` **ignoreFocusOut**: `boolean`

Set to `true` to keep the picker open when focus moves to another part of the editor or to another window.
This setting is ignored on iPad and is always false.

#### Defined in

[index.d.ts:1820](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1820)

___

### matchOnDescription

• `Optional` **matchOnDescription**: `boolean`

An optional flag to include the description when filtering the picks.

#### Defined in

[index.d.ts:1804](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1804)

___

### matchOnDetail

• `Optional` **matchOnDetail**: `boolean`

An optional flag to include the detail when filtering the picks.

#### Defined in

[index.d.ts:1809](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1809)

___

### placeHolder

• `Optional` **placeHolder**: `string`

An optional string to show as placeholder in the input box to guide the user what to pick on.

#### Defined in

[index.d.ts:1814](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1814)

___

### title

• `Optional` **title**: `string`

An optional string that represents the title of the quick pick.

#### Defined in

[index.d.ts:1799](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1799)

## Methods

### onDidSelectItem

▸ `Optional` **onDidSelectItem**(`item`): `any`

An optional function that is invoked whenever an item is selected.

#### Parameters

| Name | Type |
| :------ | :------ |
| `item` | `string` \| [`QuickPickItem`](codearts_plugin_.QuickPickItem.md) |

#### Returns

`any`

#### Defined in

[index.d.ts:1830](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1830)
