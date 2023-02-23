[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SnippetString

# Class: SnippetString

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SnippetString

A snippet string is a template which allows to insert text
and to control the editor cursor when insertion happens.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.SnippetString.md#constructor)

### Properties

- [value](cloudide_plugin_.SnippetString.md#value)

### Methods

- [appendPlaceholder](cloudide_plugin_.SnippetString.md#appendplaceholder)
- [appendTabstop](cloudide_plugin_.SnippetString.md#appendtabstop)
- [appendText](cloudide_plugin_.SnippetString.md#appendtext)
- [appendVariable](cloudide_plugin_.SnippetString.md#appendvariable)

## Constructors

### constructor

• **new SnippetString**(`value?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Defined in

[index.d.ts:547](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L547)

## Properties

### value

• **value**: `string`

The snippet string.

#### Defined in

[index.d.ts:545](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L545)

## Methods

### appendPlaceholder

▸ **appendPlaceholder**(`value`, `number?`): [`SnippetString`](cloudide_plugin_.SnippetString.md)

Builder-function that appends a placeholder (`${1:value}`) to
the [`value`](#SnippetString.value) of this snippet string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` \| (`snippet`: [`SnippetString`](cloudide_plugin_.SnippetString.md)) => `any` | The value of this placeholder - either a string or a function with which a nested snippet can be created. |
| `number?` | `number` | The number of this tabstop, defaults to an auto-increment value starting at 1. |

#### Returns

[`SnippetString`](cloudide_plugin_.SnippetString.md)

This snippet string.

#### Defined in

[index.d.ts:578](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L578)

___

### appendTabstop

▸ **appendTabstop**(`number?`): [`SnippetString`](cloudide_plugin_.SnippetString.md)

Builder-function that appends a tabstop (`$1`, `$2` etc) to
the [`value`](#SnippetString.value) of this snippet string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `number?` | `number` | The number of this tabstop, defaults to an auto-increment value starting at 1. |

#### Returns

[`SnippetString`](cloudide_plugin_.SnippetString.md)

This snippet string.

#### Defined in

[index.d.ts:566](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L566)

___

### appendText

▸ **appendText**(`string`): [`SnippetString`](cloudide_plugin_.SnippetString.md)

Builder-function that appends the given string to
the [`value`](#SnippetString.value) of this snippet string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `string` | `string` | A value to append 'as given'. The string will be escaped. |

#### Returns

[`SnippetString`](cloudide_plugin_.SnippetString.md)

This snippet string.

#### Defined in

[index.d.ts:556](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L556)

___

### appendVariable

▸ **appendVariable**(`name`, `defaultValue`): [`SnippetString`](cloudide_plugin_.SnippetString.md)

Builder-function that appends a variable (`${VAR}`) to
the [`value`](#SnippetString.value) of this snippet string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the variable - excluding the `$`. |
| `defaultValue` | `string` \| (`snippet`: [`SnippetString`](cloudide_plugin_.SnippetString.md)) => `any` | The default value which is used when the variable name cannot be resolved - either a string or a function with which a nested snippet can be created. |

#### Returns

[`SnippetString`](cloudide_plugin_.SnippetString.md)

This snippet string.

#### Defined in

[index.d.ts:589](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L589)
