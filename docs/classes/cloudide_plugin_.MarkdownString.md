[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / MarkdownString

# Class: MarkdownString

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).MarkdownString

The MarkdownString represents human readable text that supports formatting via the
markdown syntax. Standard markdown is supported, also tables, but no embedded html.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.MarkdownString.md#constructor)

### Properties

- [isTrusted](cloudide_plugin_.MarkdownString.md#istrusted)
- [value](cloudide_plugin_.MarkdownString.md#value)

### Methods

- [appendCodeblock](cloudide_plugin_.MarkdownString.md#appendcodeblock)
- [appendMarkdown](cloudide_plugin_.MarkdownString.md#appendmarkdown)
- [appendText](cloudide_plugin_.MarkdownString.md#appendtext)

## Constructors

### constructor

• **new MarkdownString**(`value?`)

Creates a new markdown string with the given value.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | Optional, initial value. |

#### Defined in

[index.d.ts:812](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L812)

## Properties

### isTrusted

• `Optional` **isTrusted**: `boolean`

Indicates that this markdown string is from a trusted source. Only *trusted*
markdown supports links that execute commands, e.g. `[Run it](command:myCommandId)`.

#### Defined in

[index.d.ts:805](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L805)

___

### value

• **value**: `string`

The markdown string.

#### Defined in

[index.d.ts:799](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L799)

## Methods

### appendCodeblock

▸ **appendCodeblock**(`value`, `language?`): [`MarkdownString`](cloudide_plugin_.MarkdownString.md)

Appends the given string as codeblock using the provided language.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | A code snippet. |
| `language?` | `string` | An optional [language identifier](#languages.getLanguages). |

#### Returns

[`MarkdownString`](cloudide_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:831](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L831)

___

### appendMarkdown

▸ **appendMarkdown**(`value`): [`MarkdownString`](cloudide_plugin_.MarkdownString.md)

Appends the given string 'as is' to this markdown string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | Markdown string. |

#### Returns

[`MarkdownString`](cloudide_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:824](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L824)

___

### appendText

▸ **appendText**(`value`): [`MarkdownString`](cloudide_plugin_.MarkdownString.md)

Appends and escapes the given string to this markdown string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | Plain text. |

#### Returns

[`MarkdownString`](cloudide_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:818](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L818)
