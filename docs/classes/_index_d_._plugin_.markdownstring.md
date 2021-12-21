**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / MarkdownString

# Class: MarkdownString

The MarkdownString represents human-readable text that supports formatting via the
markdown syntax. Standard markdown is supported, also tables, but no embedded html.

When created with `supportThemeIcons` then rendering of [theme icons](#ThemeIcon) via
the `$(<name>)`-syntax is supported.

## Hierarchy

* **MarkdownString**

## Index

### Constructors

* [constructor](_index_d_._plugin_.markdownstring.md#constructor)

### Properties

* [isTrusted](_index_d_._plugin_.markdownstring.md#istrusted)
* [supportThemeIcons](_index_d_._plugin_.markdownstring.md#supportthemeicons)
* [value](_index_d_._plugin_.markdownstring.md#value)

### Methods

* [appendCodeblock](_index_d_._plugin_.markdownstring.md#appendcodeblock)
* [appendMarkdown](_index_d_._plugin_.markdownstring.md#appendmarkdown)
* [appendText](_index_d_._plugin_.markdownstring.md#appendtext)

## Constructors

### constructor

\+ **new MarkdownString**(`value?`: string, `supportThemeIcons?`: boolean): [MarkdownString](_index_d_._plugin_.markdownstring.md)

*Defined in [index.d.ts:2650](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2650)*

Creates a new markdown string with the given value.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value?` | string | Optional, initial value. |
`supportThemeIcons?` | boolean | Optional, Specifies whether [ThemeIcons](#ThemeIcon) are supported within the [`MarkdownString`](#MarkdownString).  |

**Returns:** [MarkdownString](_index_d_._plugin_.markdownstring.md)

## Properties

### isTrusted

• `Optional` **isTrusted**: boolean

*Defined in [index.d.ts:2645](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2645)*

Indicates that this markdown string is from a trusted source. Only *trusted*
markdown supports links that execute commands, e.g. `[Run it](command:myCommandId)`.

___

### supportThemeIcons

• `Optional` `Readonly` **supportThemeIcons**: boolean

*Defined in [index.d.ts:2650](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2650)*

Indicates that this markdown string can contain [ThemeIcons](#ThemeIcon), e.g. `$(zap)`.

___

### value

•  **value**: string

*Defined in [index.d.ts:2639](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2639)*

The markdown string.

## Methods

### appendCodeblock

▸ **appendCodeblock**(`value`: string, `language?`: string): [MarkdownString](_index_d_._plugin_.markdownstring.md)

*Defined in [index.d.ts:2677](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2677)*

Appends the given string as codeblock using the provided language.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string | A code snippet. |
`language?` | string | An optional [language identifier](#languages.getLanguages).  |

**Returns:** [MarkdownString](_index_d_._plugin_.markdownstring.md)

___

### appendMarkdown

▸ **appendMarkdown**(`value`: string): [MarkdownString](_index_d_._plugin_.markdownstring.md)

*Defined in [index.d.ts:2670](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2670)*

Appends the given string 'as is' to this markdown string. When [`supportThemeIcons`](#MarkdownString.supportThemeIcons) is `true`, [ThemeIcons](#ThemeIcon) in the `value` will be iconified.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string | Markdown string.  |

**Returns:** [MarkdownString](_index_d_._plugin_.markdownstring.md)

___

### appendText

▸ **appendText**(`value`: string): [MarkdownString](_index_d_._plugin_.markdownstring.md)

*Defined in [index.d.ts:2664](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2664)*

Appends and escapes the given string to this markdown string.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string | Plain text.  |

**Returns:** [MarkdownString](_index_d_._plugin_.markdownstring.md)
