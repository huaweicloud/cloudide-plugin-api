[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / LanguageStatusItem

# Interface: LanguageStatusItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).LanguageStatusItem

A language status item is the preferred way to present language status reports for the active text editors,
such as selected linter or notifying about a configuration problem.

## Table of contents

### Properties

- [accessibilityInformation](codearts_plugin_.LanguageStatusItem.md#accessibilityinformation)
- [busy](codearts_plugin_.LanguageStatusItem.md#busy)
- [command](codearts_plugin_.LanguageStatusItem.md#command)
- [detail](codearts_plugin_.LanguageStatusItem.md#detail)
- [id](codearts_plugin_.LanguageStatusItem.md#id)
- [name](codearts_plugin_.LanguageStatusItem.md#name)
- [selector](codearts_plugin_.LanguageStatusItem.md#selector)
- [severity](codearts_plugin_.LanguageStatusItem.md#severity)
- [text](codearts_plugin_.LanguageStatusItem.md#text)

### Methods

- [dispose](codearts_plugin_.LanguageStatusItem.md#dispose)

## Properties

### accessibilityInformation

• `Optional` **accessibilityInformation**: [`AccessibilityInformation`](codearts_plugin_.AccessibilityInformation.md)

Accessibility information used when a screen reader interacts with this item

#### Defined in

[index.d.ts:6136](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6136)

___

### busy

• **busy**: `boolean`

Controls whether the item is shown as "busy". Defaults to `false`.

#### Defined in

[index.d.ts:6126](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6126)

___

### command

• **command**: `undefined` \| [`Command`](codearts_plugin_.Command.md)

A [`command`](codearts_plugin_.Command.md) for this item.

#### Defined in

[index.d.ts:6131](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6131)

___

### detail

• `Optional` **detail**: `string`

Optional, human-readable details for this item.

#### Defined in

[index.d.ts:6121](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6121)

___

### id

• `Readonly` **id**: `string`

The identifier of this item.

#### Defined in

[index.d.ts:6086](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6086)

___

### name

• **name**: `undefined` \| `string`

The short name of this item, like 'Java Language Status', etc.

#### Defined in

[index.d.ts:6091](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6091)

___

### selector

• **selector**: [`DocumentSelector`](../modules/_codearts_plugin_.md#documentselector)

A [selector](../modules/_codearts_plugin_.md#documentselector) that defines for what editors
this item shows.

#### Defined in

[index.d.ts:6097](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6097)

___

### severity

• **severity**: [`LanguageStatusSeverity`](../enums/codearts_plugin_.LanguageStatusSeverity.md)

The severity of this item.

Defaults to [information](../enums/codearts_plugin_.LanguageStatusSeverity.md#information). You can use this property to
signal to users that there is a problem that needs attention, like a missing executable or an
invalid configuration.

#### Defined in

[index.d.ts:6106](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6106)

___

### text

• **text**: `string`

The text to show for the entry. You can embed icons in the text by leveraging the syntax:

`My text $(icon-name) contains icons like $(icon-name) this one.`

Where the icon-name is taken from the ThemeIcon [icon set](https://code.visualstudio.com/api/references/icons-in-labels#icon-listing), e.g.
`light-bulb`, `thumbsup`, `zap` etc.

#### Defined in

[index.d.ts:6116](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6116)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose and free associated resources.

#### Returns

`void`

#### Defined in

[index.d.ts:6141](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6141)
