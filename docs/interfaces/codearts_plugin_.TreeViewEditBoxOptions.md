[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TreeViewEditBoxOptions

# Interface: TreeViewEditBoxOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).TreeViewEditBoxOptions

## Table of contents

### Properties

- [onAccept](codearts_plugin_.TreeViewEditBoxOptions.md#onaccept)
- [placeholder](codearts_plugin_.TreeViewEditBoxOptions.md#placeholder)
- [rootPath](codearts_plugin_.TreeViewEditBoxOptions.md#rootpath)
- [tooltip](codearts_plugin_.TreeViewEditBoxOptions.md#tooltip)
- [validateInput](codearts_plugin_.TreeViewEditBoxOptions.md#validateinput)
- [value](codearts_plugin_.TreeViewEditBoxOptions.md#value)
- [valueSelection](codearts_plugin_.TreeViewEditBoxOptions.md#valueselection)

## Properties

### onAccept

• `Optional` **onAccept**: (`value`: `string`) => [`Thenable`](Thenable.md)<`void`\>

#### Type declaration

▸ (`value`): [`Thenable`](Thenable.md)<`void`\>

The processing function when receiving the edited value.
onAccept is used to handle the situation that a node is refreshed for a long time. I need to keep only one node editing and its editing state.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | value of the input box when finish edit. |

##### Returns

[`Thenable`](Thenable.md)<`void`\>

A Thenable deal with accepted value.

#### Defined in

[index.d.ts:11090](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L11090)

___

### placeholder

• `Optional` **placeholder**: `string`

An optional string to show as placeholder in the input box to guide the user what to type.

#### Defined in

[index.d.ts:11044](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L11044)

___

### rootPath

• `Optional` **rootPath**: [`Uri`](../classes/codearts_plugin_.Uri.md)

If the treeItem contains a resourceUri, the root path can be determined so we know the full path when creating a new node.
it Required for the first level TreeItem containing resourceUri.

#### Defined in

[index.d.ts:11070](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L11070)

___

### tooltip

• `Optional` **tooltip**: (`value`: `string`, `path?`: `string`) => `undefined` \| `string` \| [`MarkdownString`](../classes/codearts_plugin_.MarkdownString.md)

#### Type declaration

▸ (`value`, `path?`): `undefined` \| `string` \| [`MarkdownString`](../classes/codearts_plugin_.MarkdownString.md)

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | Value of the current text box. |
| `path?` | `string` | If TreeItem contains resourceUri, it is the fsPath of the edited Uri. The tooltip text when you hover over this item. [["tooltip"]](../classes/codearts_plugin_.TreeItem.md) |

##### Returns

`undefined` \| `string` \| [`MarkdownString`](../classes/codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:11064](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L11064)

___

### validateInput

• `Optional` **validateInput**: (`value`: `string`, `isAcceptEvent`: `boolean`) => `undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md) \| [`Thenable`](Thenable.md)<`undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)\>

#### Type declaration

▸ (`value`, `isAcceptEvent`): `undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md) \| [`Thenable`](Thenable.md)<`undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)\>

An optional function that will be called to validate input and to give a hint
to the user.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | The current value of the input box. |
| `isAcceptEvent` | `boolean` | Whether this validation is triggered by the accept or change event. |

##### Returns

`undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md) \| [`Thenable`](Thenable.md)<`undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)\>

[InputBoxValidationMessage](codearts_plugin_.InputBoxValidationMessage.md) which can provide a specific message severity.
  Return `undefined`, `null`, or the empty string when 'value' is valid.

#### Defined in

[index.d.ts:11081](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L11081)

___

### value

• `Optional` **value**: `string`

The value to prefill in the input box.

#### Defined in

[index.d.ts:11049](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L11049)

___

### valueSelection

• `Optional` **valueSelection**: [`number`, `number`]

Selection of the prefilled [`value`](#TreeViewEditBoxOptions.value). Defined as tuple of two number where the
first is the inclusive start index and the second the exclusive end index. When `undefined` the whole
word will be selected, when empty (start equals end) only the cursor will be set,
otherwise the defined range will be selected.

#### Defined in

[index.d.ts:11057](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L11057)
