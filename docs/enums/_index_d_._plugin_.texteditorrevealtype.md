**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextEditorRevealType

# Enumeration: TextEditorRevealType

Represents different [reveal](#TextEditor.revealRange) strategies in a text editor.

## Index

### Enumeration members

* [AtTop](_index_d_._plugin_.texteditorrevealtype.md#attop)
* [Default](_index_d_._plugin_.texteditorrevealtype.md#default)
* [InCenter](_index_d_._plugin_.texteditorrevealtype.md#incenter)
* [InCenterIfOutsideViewport](_index_d_._plugin_.texteditorrevealtype.md#incenterifoutsideviewport)

## Enumeration members

### AtTop

•  **AtTop**:  = 3

*Defined in [index.d.ts:834](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L834)*

The range will always be revealed at the top of the viewport.

___

### Default

•  **Default**:  = 0

*Defined in [index.d.ts:821](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L821)*

The range will be revealed with as little scrolling as possible.

___

### InCenter

•  **InCenter**:  = 1

*Defined in [index.d.ts:825](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L825)*

The range will always be revealed in the center of the viewport.

___

### InCenterIfOutsideViewport

•  **InCenterIfOutsideViewport**:  = 2

*Defined in [index.d.ts:830](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L830)*

If the range is outside the viewport, it will be revealed in the center of the viewport.
Otherwise, it will be revealed with as little scrolling as possible.
