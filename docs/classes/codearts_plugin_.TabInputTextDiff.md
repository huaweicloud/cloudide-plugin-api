[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TabInputTextDiff

# Class: TabInputTextDiff

["@codearts/plugin"](../modules/_codearts_plugin_.md).TabInputTextDiff

The tab represents two text based resources
being rendered as a diff.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TabInputTextDiff.md#constructor)

### Properties

- [modified](codearts_plugin_.TabInputTextDiff.md#modified)
- [original](codearts_plugin_.TabInputTextDiff.md#original)

## Constructors

### constructor

• **new TabInputTextDiff**(`original`, `modified`)

Constructs a new text diff tab input with the given URIs.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `original` | [`Uri`](codearts_plugin_.Uri.md) | The uri of the original text resource. |
| `modified` | [`Uri`](codearts_plugin_.Uri.md) | The uri of the modified text resource. |

#### Defined in

[index.d.ts:17149](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17149)

## Properties

### modified

• `Readonly` **modified**: [`Uri`](codearts_plugin_.Uri.md)

The uri of the modified text resource.

#### Defined in

[index.d.ts:17143](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17143)

___

### original

• `Readonly` **original**: [`Uri`](codearts_plugin_.Uri.md)

The uri of the original text resource.

#### Defined in

[index.d.ts:17139](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17139)
