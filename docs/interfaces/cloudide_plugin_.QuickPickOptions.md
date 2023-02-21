[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / QuickPickOptions

# Interface: QuickPickOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).QuickPickOptions

Options for configuration behavior of the quick pick

## Table of contents

### Properties

- [canPickMany](cloudide_plugin_.QuickPickOptions.md#canpickmany)
- [ignoreFocusOut](cloudide_plugin_.QuickPickOptions.md#ignorefocusout)
- [matchOnDescription](cloudide_plugin_.QuickPickOptions.md#matchondescription)
- [matchOnDetail](cloudide_plugin_.QuickPickOptions.md#matchondetail)
- [placeHolder](cloudide_plugin_.QuickPickOptions.md#placeholder)

### Methods

- [onDidSelectItem](cloudide_plugin_.QuickPickOptions.md#ondidselectitem)

## Properties

### canPickMany

• `Optional` **canPickMany**: `boolean`

If `true` make picker accept multiple selections.
Not implemented yet

#### Defined in

[index.d.ts:2292](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2292)

___

### ignoreFocusOut

• `Optional` **ignoreFocusOut**: `boolean`

If `true` prevent picker closing when it's loses focus

#### Defined in

[index.d.ts:2286](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2286)

___

### matchOnDescription

• `Optional` **matchOnDescription**: `boolean`

A flag to include the description when filtering

#### Defined in

[index.d.ts:2271](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2271)

___

### matchOnDetail

• `Optional` **matchOnDetail**: `boolean`

A flag to include the detail when filtering

#### Defined in

[index.d.ts:2276](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2276)

___

### placeHolder

• `Optional` **placeHolder**: `string`

The place holder in input box

#### Defined in

[index.d.ts:2281](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2281)

## Methods

### onDidSelectItem

▸ `Optional` **onDidSelectItem**(`item`): `any`

Function that is invoked when item selected

#### Parameters

| Name | Type |
| :------ | :------ |
| `item` | `string` \| [`QuickPickItem`](cloudide_plugin_.QuickPickItem.md) |

#### Returns

`any`

#### Defined in

[index.d.ts:2297](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2297)
