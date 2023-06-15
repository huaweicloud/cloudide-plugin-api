[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineValueVariableLookup

# Class: InlineValueVariableLookup

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineValueVariableLookup

Provide inline value through a variable lookup.
If only a range is specified, the variable name will be extracted from the underlying document.
An optional variable name can be used to override the extracted name.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.InlineValueVariableLookup.md#constructor)

### Properties

- [caseSensitiveLookup](codearts_plugin_.InlineValueVariableLookup.md#casesensitivelookup)
- [range](codearts_plugin_.InlineValueVariableLookup.md#range)
- [variableName](codearts_plugin_.InlineValueVariableLookup.md#variablename)

## Constructors

### constructor

• **new InlineValueVariableLookup**(`range`, `variableName?`, `caseSensitiveLookup?`)

Creates a new InlineValueVariableLookup object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The document line where to show the inline value. |
| `variableName?` | `string` | The name of the variable to look up. |
| `caseSensitiveLookup?` | `boolean` | How to perform the lookup. If missing lookup is case sensitive. |

#### Defined in

[index.d.ts:2973](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L2973)

## Properties

### caseSensitiveLookup

• `Readonly` **caseSensitiveLookup**: `boolean`

How to perform the lookup.

#### Defined in

[index.d.ts:2965](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L2965)

___

### range

• `Readonly` **range**: [`Range`](codearts_plugin_.Range.md)

The document range for which the inline value applies.
The range is used to extract the variable name from the underlying document.

#### Defined in

[index.d.ts:2957](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L2957)

___

### variableName

• `Optional` `Readonly` **variableName**: `string`

If specified the name of the variable to look up.

#### Defined in

[index.d.ts:2961](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L2961)
