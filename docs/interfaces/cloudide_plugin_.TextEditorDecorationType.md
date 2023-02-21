[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextEditorDecorationType

# Interface: TextEditorDecorationType

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextEditorDecorationType

Represents a handle to a set of decorations
sharing the same [styling options](#DecorationRenderOptions) in a [text editor](#TextEditor).

To get an instance of a `TextEditorDecorationType` use
[createTextEditorDecorationType](#window.createTextEditorDecorationType).

## Table of contents

### Properties

- [key](cloudide_plugin_.TextEditorDecorationType.md#key)

### Methods

- [dispose](cloudide_plugin_.TextEditorDecorationType.md#dispose)

## Properties

### key

• `Readonly` **key**: `string`

Internal representation of the handle.

#### Defined in

[index.d.ts:668](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L668)

## Methods

### dispose

▸ **dispose**(): `void`

Remove this decoration type and all decorations on all text editors using it.

#### Returns

`void`

#### Defined in

[index.d.ts:673](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L673)
