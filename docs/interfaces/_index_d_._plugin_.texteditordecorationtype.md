**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextEditorDecorationType

# Interface: TextEditorDecorationType

Represents a handle to a set of decorations
sharing the same [styling options](#DecorationRenderOptions) in a [text editor](#TextEditor).

To get an instance of a `TextEditorDecorationType` use
[createTextEditorDecorationType](#window.createTextEditorDecorationType).

## Hierarchy

* **TextEditorDecorationType**

## Index

### Properties

* [key](_index_d_._plugin_.texteditordecorationtype.md#key)

### Methods

* [dispose](_index_d_._plugin_.texteditordecorationtype.md#dispose)

## Properties

### key

• `Readonly` **key**: string

*Defined in [index.d.ts:693](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L693)*

Internal representation of the handle.

## Methods

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:698](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L698)*

Remove this decoration type and all decorations on all text editors using it.

**Returns:** void
