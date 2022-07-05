[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / MarkdownString

# Class: MarkdownString

["@codearts/plugin"](../modules/_codearts_plugin_.md).MarkdownString

## Table of contents

### Constructors

- [constructor](codearts_plugin_.MarkdownString.md#constructor)

### Properties

- [baseUri](codearts_plugin_.MarkdownString.md#baseuri)
- [isTrusted](codearts_plugin_.MarkdownString.md#istrusted)
- [supportHtml](codearts_plugin_.MarkdownString.md#supporthtml)
- [supportThemeIcons](codearts_plugin_.MarkdownString.md#supportthemeicons)
- [value](codearts_plugin_.MarkdownString.md#value)

### Methods

- [appendCodeblock](codearts_plugin_.MarkdownString.md#appendcodeblock)
- [appendMarkdown](codearts_plugin_.MarkdownString.md#appendmarkdown)
- [appendText](codearts_plugin_.MarkdownString.md#appendtext)

## Constructors

### constructor

• **new MarkdownString**(`value?`, `supportThemeIcons?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` |  |
| `supportThemeIcons?` | `boolean` |  |

#### Defined in

[index.d.ts:2799](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2799)

## Properties

### baseUri

• `Optional` **baseUri**: [`Uri`](codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:2791](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2791)

___

### isTrusted

• `Optional` **isTrusted**: `boolean`

#### Defined in

[index.d.ts:2753](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2753)

___

### supportHtml

• `Optional` **supportHtml**: `boolean`

#### Defined in

[index.d.ts:2770](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2770)

___

### supportThemeIcons

• `Optional` **supportThemeIcons**: `boolean`

#### Defined in

[index.d.ts:2758](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2758)

___

### value

• **value**: `string`

#### Defined in

[index.d.ts:2747](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2747)

## Methods

### appendCodeblock

▸ **appendCodeblock**(`value`, `language?`): [`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` |  |
| `language?` | `string` |  |

#### Returns

[`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:2818](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2818)

___

### appendMarkdown

▸ **appendMarkdown**(`value`): [`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` |  |

#### Returns

[`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:2811](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2811)

___

### appendText

▸ **appendText**(`value`): [`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` |  |

#### Returns

[`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:2805](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2805)
