[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Tab

# Interface: Tab

["@codearts/plugin"](../modules/_codearts_plugin_.md).Tab

Represents a tab within a [group of tabs](codearts_plugin_.TabGroup.md).
Tabs are merely the graphical representation within the editor area.
A backing editor is not a guarantee.

## Table of contents

### Properties

- [group](codearts_plugin_.Tab.md#group)
- [input](codearts_plugin_.Tab.md#input)
- [isActive](codearts_plugin_.Tab.md#isactive)
- [isDirty](codearts_plugin_.Tab.md#isdirty)
- [isPinned](codearts_plugin_.Tab.md#ispinned)
- [isPreview](codearts_plugin_.Tab.md#ispreview)
- [label](codearts_plugin_.Tab.md#label)

## Properties

### group

• `Readonly` **group**: [`TabGroup`](codearts_plugin_.TabGroup.md)

The group which the tab belongs to.

#### Defined in

[index.d.ts:16046](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L16046)

___

### input

• `Readonly` **input**: `unknown`

Defines the structure of the tab i.e. text, notebook, custom, etc.
Resource and other useful properties are defined on the tab kind.

#### Defined in

[index.d.ts:16052](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L16052)

___

### isActive

• `Readonly` **isActive**: `boolean`

Whether or not the tab is currently active.
This is dictated by being the selected tab in the group.

#### Defined in

[index.d.ts:16058](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L16058)

___

### isDirty

• `Readonly` **isDirty**: `boolean`

Whether or not the dirty indicator is present on the tab.

#### Defined in

[index.d.ts:16063](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L16063)

___

### isPinned

• `Readonly` **isPinned**: `boolean`

Whether or not the tab is pinned (pin icon is present).

#### Defined in

[index.d.ts:16068](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L16068)

___

### isPreview

• `Readonly` **isPreview**: `boolean`

Whether or not the tab is in preview mode.

#### Defined in

[index.d.ts:16073](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L16073)

___

### label

• `Readonly` **label**: `string`

The text displayed on the tab.

#### Defined in

[index.d.ts:16041](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L16041)
