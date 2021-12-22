**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SnippetString

# Class: SnippetString

A snippet string is a template which allows to insert text
and to control the editor cursor when insertion happens.

A snippet can define tab stops and placeholders with `$1`, `$2`
and `${3:foo}`. `$0` defines the final tab stop, it defaults to
the end of the snippet. Variables are defined with `$name` and
`${name:default value}`. The full snippet syntax is documented
[here](https://code.visualstudio.com/docs/editor/userdefinedsnippets#_creating-your-own-snippets).

## Hierarchy

* **SnippetString**

## Index

### Constructors

* [constructor](_index_d_._plugin_.snippetstring.md#constructor)

### Properties

* [value](_index_d_._plugin_.snippetstring.md#value)

### Methods

* [appendChoice](_index_d_._plugin_.snippetstring.md#appendchoice)
* [appendPlaceholder](_index_d_._plugin_.snippetstring.md#appendplaceholder)
* [appendTabstop](_index_d_._plugin_.snippetstring.md#appendtabstop)
* [appendText](_index_d_._plugin_.snippetstring.md#appendtext)
* [appendVariable](_index_d_._plugin_.snippetstring.md#appendvariable)

## Constructors

### constructor

\+ **new SnippetString**(`value?`: string): [SnippetString](_index_d_._plugin_.snippetstring.md)

*Defined in [index.d.ts:3320](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3320)*

#### Parameters:

Name | Type |
------ | ------ |
`value?` | string |

**Returns:** [SnippetString](_index_d_._plugin_.snippetstring.md)

## Properties

### value

•  **value**: string

*Defined in [index.d.ts:3320](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3320)*

The snippet string.

## Methods

### appendChoice

▸ **appendChoice**(`values`: string[], `number?`: number): [SnippetString](_index_d_._plugin_.snippetstring.md)

*Defined in [index.d.ts:3364](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3364)*

Builder-function that appends a choice (`${1|a,b,c}`) to
the [`value`](#SnippetString.value) of this snippet string.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`values` | string[] | The values for choices - the array of strings |
`number?` | number | The number of this tabstop, defaults to an auto-increment value starting at 1. |

**Returns:** [SnippetString](_index_d_._plugin_.snippetstring.md)

This snippet string.

___

### appendPlaceholder

▸ **appendPlaceholder**(`value`: string \| (snippet: [SnippetString](_index_d_._plugin_.snippetstring.md)) => any, `number?`: number): [SnippetString](_index_d_._plugin_.snippetstring.md)

*Defined in [index.d.ts:3353](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3353)*

Builder-function that appends a placeholder (`${1:value}`) to
the [`value`](#SnippetString.value) of this snippet string.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string \| (snippet: [SnippetString](_index_d_._plugin_.snippetstring.md)) => any | The value of this placeholder - either a string or a function with which a nested snippet can be created. |
`number?` | number | The number of this tabstop, defaults to an auto-increment value starting at 1. |

**Returns:** [SnippetString](_index_d_._plugin_.snippetstring.md)

This snippet string.

___

### appendTabstop

▸ **appendTabstop**(`number?`: number): [SnippetString](_index_d_._plugin_.snippetstring.md)

*Defined in [index.d.ts:3341](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3341)*

Builder-function that appends a tabstop (`$1`, `$2` etc) to
the [`value`](#SnippetString.value) of this snippet string.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`number?` | number | The number of this tabstop, defaults to an auto-increment value starting at 1. |

**Returns:** [SnippetString](_index_d_._plugin_.snippetstring.md)

This snippet string.

___

### appendText

▸ **appendText**(`string`: string): [SnippetString](_index_d_._plugin_.snippetstring.md)

*Defined in [index.d.ts:3331](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3331)*

Builder-function that appends the given string to
the [`value`](#SnippetString.value) of this snippet string.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`string` | string | A value to append 'as given'. The string will be escaped. |

**Returns:** [SnippetString](_index_d_._plugin_.snippetstring.md)

This snippet string.

___

### appendVariable

▸ **appendVariable**(`name`: string, `defaultValue`: string \| (snippet: [SnippetString](_index_d_._plugin_.snippetstring.md)) => any): [SnippetString](_index_d_._plugin_.snippetstring.md)

*Defined in [index.d.ts:3375](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3375)*

Builder-function that appends a variable (`${VAR}`) to
the [`value`](#SnippetString.value) of this snippet string.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`name` | string | The name of the variable - excluding the `$`. |
`defaultValue` | string \| (snippet: [SnippetString](_index_d_._plugin_.snippetstring.md)) => any | The default value which is used when the variable name cannot be resolved - either a string or a function with which a nested snippet can be created. |

**Returns:** [SnippetString](_index_d_._plugin_.snippetstring.md)

This snippet string.
