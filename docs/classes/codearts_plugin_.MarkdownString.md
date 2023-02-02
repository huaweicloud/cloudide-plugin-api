[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / MarkdownString

# Class: MarkdownString

["@codearts/plugin"](../modules/_codearts_plugin_.md).MarkdownString

Human-readable text that supports formatting via the [markdown syntax](https://commonmark.org).

Rendering of [theme icons](codearts_plugin_.ThemeIcon.md) via the `$(<name>)`-syntax is supported
when the [`supportThemeIcons`](codearts_plugin_.MarkdownString.md#supportthemeicons) is set to `true`.

Rendering of embedded html is supported when [`supportHtml`](codearts_plugin_.MarkdownString.md#supporthtml) is set to `true`.

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

Creates a new markdown string with the given value.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | Optional, initial value. |
| `supportThemeIcons?` | `boolean` | Optional, Specifies whether [ThemeIcons](codearts_plugin_.ThemeIcon.md) are supported within the [`MarkdownString`](codearts_plugin_.MarkdownString.md). |

#### Defined in

[index.d.ts:2799](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2799)

## Properties

### baseUri

• `Optional` **baseUri**: [`Uri`](codearts_plugin_.Uri.md)

Uri that relative paths are resolved relative to.

If the `baseUri` ends with `/`, it is considered a directory and relative paths in the markdown are resolved relative to that directory:

```ts
const md = new vscode.MarkdownString(`[link](./file.js)`);
md.baseUri = vscode.Uri.file('/path/to/dir/');
// Here 'link' in the rendered markdown resolves to '/path/to/dir/file.js'
```

If the `baseUri` is a file, relative paths in the markdown are resolved relative to the parent dir of that file:

```ts
const md = new vscode.MarkdownString(`[link](./file.js)`);
md.baseUri = vscode.Uri.file('/path/to/otherFile.js');
// Here 'link' in the rendered markdown resolves to '/path/to/file.js'
```

#### Defined in

[index.d.ts:2791](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2791)

___

### isTrusted

• `Optional` **isTrusted**: `boolean`

Indicates that this markdown string is from a trusted source. Only *trusted*
markdown supports links that execute commands, e.g. `[Run it](command:myCommandId)`.

#### Defined in

[index.d.ts:2753](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2753)

___

### supportHtml

• `Optional` **supportHtml**: `boolean`

Indicates that this markdown string can contain raw html tags. Defaults to `false`.

When `supportHtml` is false, the markdown renderer will strip out any raw html tags
that appear in the markdown text. This means you can only use markdown syntax for rendering.

When `supportHtml` is true, the markdown render will also allow a safe subset of html tags
and attributes to be rendered. See https://github.com/microsoft/vscode/blob/6d2920473c6f13759c978dd89104c4270a83422d/src/vs/base/browser/markdownRenderer.ts#L296
for a list of all supported tags and attributes.

#### Defined in

[index.d.ts:2770](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2770)

___

### supportThemeIcons

• `Optional` **supportThemeIcons**: `boolean`

Indicates that this markdown string can contain [ThemeIcons](codearts_plugin_.ThemeIcon.md), e.g. `$(zap)`.

#### Defined in

[index.d.ts:2758](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2758)

___

### value

• **value**: `string`

The markdown string.

#### Defined in

[index.d.ts:2747](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2747)

## Methods

### appendCodeblock

▸ **appendCodeblock**(`value`, `language?`): [`MarkdownString`](codearts_plugin_.MarkdownString.md)

Appends the given string as codeblock using the provided language.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | A code snippet. |
| `language?` | `string` | An optional [language identifier](../modules/codearts_plugin_.languages.md#getlanguages). |

#### Returns

[`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:2818](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2818)

___

### appendMarkdown

▸ **appendMarkdown**(`value`): [`MarkdownString`](codearts_plugin_.MarkdownString.md)

Appends the given string 'as is' to this markdown string. When [`supportThemeIcons`](codearts_plugin_.MarkdownString.md#supportthemeicons) is `true`, [ThemeIcons](codearts_plugin_.ThemeIcon.md) in the `value` will be iconified.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | Markdown string. |

#### Returns

[`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:2811](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2811)

___

### appendText

▸ **appendText**(`value`): [`MarkdownString`](codearts_plugin_.MarkdownString.md)

Appends and escapes the given string to this markdown string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | Plain text. |

#### Returns

[`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:2805](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2805)
