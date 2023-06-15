[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SnippetString

# Class: SnippetString

["@codearts/plugin"](../modules/_codearts_plugin_.md).SnippetString

A snippet string is a template which allows to insert text
and to control the editor cursor when insertion happens.

A snippet can define tab stops and placeholders with `$1`, `$2`
and `${3:foo}`. `$0` defines the final tab stop, it defaults to
the end of the snippet. Variables are defined with `$name` and
`${name:default value}`. Also see
[the full snippet syntax](https://code.visualstudio.com/docs/editor/userdefinedsnippets#_creating-your-own-snippets).

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SnippetString.md#constructor)

### Properties

- [value](codearts_plugin_.SnippetString.md#value)

### Methods

- [appendChoice](codearts_plugin_.SnippetString.md#appendchoice)
- [appendPlaceholder](codearts_plugin_.SnippetString.md#appendplaceholder)
- [appendTabstop](codearts_plugin_.SnippetString.md#appendtabstop)
- [appendText](codearts_plugin_.SnippetString.md#appendtext)
- [appendVariable](codearts_plugin_.SnippetString.md#appendvariable)

## Constructors

### constructor

• **new SnippetString**(`value?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Defined in

[index.d.ts:3588](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L3588)

## Properties

### value

• **value**: `string`

The snippet string.

#### Defined in

[index.d.ts:3586](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L3586)

## Methods

### appendChoice

▸ **appendChoice**(`values`, `number?`): [`SnippetString`](codearts_plugin_.SnippetString.md)

Builder-function that appends a choice (`${1|a,b,c|}`) to
the [`value`](codearts_plugin_.SnippetString.md#value) of this snippet string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `values` | readonly `string`[] | The values for choices - the array of strings |
| `number?` | `number` | The number of this tabstop, defaults to an auto-increment value starting at 1. |

#### Returns

[`SnippetString`](codearts_plugin_.SnippetString.md)

This snippet string.

#### Defined in

[index.d.ts:3630](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L3630)

___

### appendPlaceholder

▸ **appendPlaceholder**(`value`, `number?`): [`SnippetString`](codearts_plugin_.SnippetString.md)

Builder-function that appends a placeholder (`${1:value}`) to
the [`value`](codearts_plugin_.SnippetString.md#value) of this snippet string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` \| (`snippet`: [`SnippetString`](codearts_plugin_.SnippetString.md)) => `any` | The value of this placeholder - either a string or a function with which a nested snippet can be created. |
| `number?` | `number` | The number of this tabstop, defaults to an auto-increment value starting at 1. |

#### Returns

[`SnippetString`](codearts_plugin_.SnippetString.md)

This snippet string.

#### Defined in

[index.d.ts:3619](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L3619)

___

### appendTabstop

▸ **appendTabstop**(`number?`): [`SnippetString`](codearts_plugin_.SnippetString.md)

Builder-function that appends a tabstop (`$1`, `$2` etc) to
the [`value`](codearts_plugin_.SnippetString.md#value) of this snippet string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `number?` | `number` | The number of this tabstop, defaults to an auto-increment value starting at 1. |

#### Returns

[`SnippetString`](codearts_plugin_.SnippetString.md)

This snippet string.

#### Defined in

[index.d.ts:3607](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L3607)

___

### appendText

▸ **appendText**(`string`): [`SnippetString`](codearts_plugin_.SnippetString.md)

Builder-function that appends the given string to
the [`value`](codearts_plugin_.SnippetString.md#value) of this snippet string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `string` | `string` | A value to append 'as given'. The string will be escaped. |

#### Returns

[`SnippetString`](codearts_plugin_.SnippetString.md)

This snippet string.

#### Defined in

[index.d.ts:3597](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L3597)

___

### appendVariable

▸ **appendVariable**(`name`, `defaultValue`): [`SnippetString`](codearts_plugin_.SnippetString.md)

Builder-function that appends a variable (`${VAR}`) to
the [`value`](codearts_plugin_.SnippetString.md#value) of this snippet string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the variable - excluding the `$`. |
| `defaultValue` | `string` \| (`snippet`: [`SnippetString`](codearts_plugin_.SnippetString.md)) => `any` | The default value which is used when the variable name cannot be resolved - either a string or a function with which a nested snippet can be created. |

#### Returns

[`SnippetString`](codearts_plugin_.SnippetString.md)

This snippet string.

#### Defined in

[index.d.ts:3641](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L3641)
