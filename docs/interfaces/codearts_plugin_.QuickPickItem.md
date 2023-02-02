[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / QuickPickItem

# Interface: QuickPickItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).QuickPickItem

Represents an item that can be selected from
a list of items.

## Table of contents

### Properties

- [alwaysShow](codearts_plugin_.QuickPickItem.md#alwaysshow)
- [buttons](codearts_plugin_.QuickPickItem.md#buttons)
- [description](codearts_plugin_.QuickPickItem.md#description)
- [detail](codearts_plugin_.QuickPickItem.md#detail)
- [kind](codearts_plugin_.QuickPickItem.md#kind)
- [label](codearts_plugin_.QuickPickItem.md#label)
- [picked](codearts_plugin_.QuickPickItem.md#picked)

## Properties

### alwaysShow

• `Optional` **alwaysShow**: `boolean`

Always show this item.

Note: this property is ignored when [kind](codearts_plugin_.QuickPickItem.md#kind) is set to [Separator](../enums/codearts_plugin_.QuickPickItemKind.md#separator)

#### Defined in

[index.d.ts:1778](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1778)

___

### buttons

• `Optional` **buttons**: readonly [`QuickInputButton`](codearts_plugin_.QuickInputButton.md)[]

Optional buttons that will be rendered on this particular item. These buttons will trigger
an [QuickPickItemButtonEvent](codearts_plugin_.QuickPickItemButtonEvent.md) when clicked. Buttons are only rendered when using a quickpick
created by the [()](../modules/codearts_plugin_.window.md#createquickpick) API. Buttons are not rendered when using
the [()](../modules/codearts_plugin_.window.md#showquickpick) API.

Note: this property is ignored when [kind](codearts_plugin_.QuickPickItem.md#kind) is set to [Separator](../enums/codearts_plugin_.QuickPickItemKind.md#separator)

#### Defined in

[index.d.ts:1788](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1788)

___

### description

• `Optional` **description**: `string`

A human-readable string which is rendered less prominent in the same line. Supports rendering of
[theme icons](../classes/codearts_plugin_.ThemeIcon.md) via the `$(<name>)`-syntax.

Note: this property is ignored when [kind](codearts_plugin_.QuickPickItem.md#kind) is set to [Separator](../enums/codearts_plugin_.QuickPickItemKind.md#separator)

#### Defined in

[index.d.ts:1751](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1751)

___

### detail

• `Optional` **detail**: `string`

A human-readable string which is rendered less prominent in a separate line. Supports rendering of
[theme icons](../classes/codearts_plugin_.ThemeIcon.md) via the `$(<name>)`-syntax.

Note: this property is ignored when [kind](codearts_plugin_.QuickPickItem.md#kind) is set to [Separator](../enums/codearts_plugin_.QuickPickItemKind.md#separator)

#### Defined in

[index.d.ts:1759](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1759)

___

### kind

• `Optional` **kind**: [`QuickPickItemKind`](../enums/codearts_plugin_.QuickPickItemKind.md)

The kind of QuickPickItem that will determine how this item is rendered in the quick pick. When not specified,
the default is [Default](../enums/codearts_plugin_.QuickPickItemKind.md#default).

#### Defined in

[index.d.ts:1743](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1743)

___

### label

• **label**: `string`

A human-readable string which is rendered prominent. Supports rendering of [theme icons](../classes/codearts_plugin_.ThemeIcon.md) via
the `$(<name>)`-syntax.

#### Defined in

[index.d.ts:1737](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1737)

___

### picked

• `Optional` **picked**: `boolean`

Optional flag indicating if this item is picked initially. This is only honored when using
the [()](../modules/codearts_plugin_.window.md#showquickpick) API. To do the same thing with the [()](../modules/codearts_plugin_.window.md#createquickpick) API,
simply set the [selectedItems](codearts_plugin_.QuickPick.md#selecteditems) to the items you want picked initially.
(*Note:* This is only honored when the picker allows multiple selections.)

**`See`**

[canPickMany](codearts_plugin_.QuickPickOptions.md#canpickmany)

Note: this property is ignored when [kind](codearts_plugin_.QuickPickItem.md#kind) is set to [Separator](../enums/codearts_plugin_.QuickPickItemKind.md#separator)

#### Defined in

[index.d.ts:1771](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1771)
