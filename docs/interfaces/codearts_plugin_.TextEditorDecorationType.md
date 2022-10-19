[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditorDecorationType

# Interface: TextEditorDecorationType

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditorDecorationType

Represents a handle to a set of decorations
sharing the same [styling options](codearts_plugin_.DecorationRenderOptions.md) in a [text editor](codearts_plugin_.TextEditor.md).

To get an instance of a `TextEditorDecorationType` use
[createTextEditorDecorationType](../modules/codearts_plugin_.window.md#createtexteditordecorationtype).

## Table of contents

### Properties

- [key](codearts_plugin_.TextEditorDecorationType.md#key)

### Methods

- [dispose](codearts_plugin_.TextEditorDecorationType.md#dispose)

## Properties

### key

• `Readonly` **key**: `string`

Internal representation of the handle.

#### Defined in

[index.d.ts:693](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L693)

## Methods

### dispose

▸ **dispose**(): `void`

Remove this decoration type and all decorations on all text editors using it.

#### Returns

`void`

#### Defined in

[index.d.ts:698](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L698)
