[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / WebviewPanelShowOptions

# Interface: WebviewPanelShowOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).WebviewPanelShowOptions

Settings to determine where webview panel will be reside

## Table of contents

### Properties

- [area](cloudide_plugin_.WebviewPanelShowOptions.md#area)
- [preserveFocus](cloudide_plugin_.WebviewPanelShowOptions.md#preservefocus)
- [viewColumn](cloudide_plugin_.WebviewPanelShowOptions.md#viewcolumn)

## Properties

### area

• `Optional` **area**: [`WebviewPanelTargetArea`](../enums/cloudide_plugin_.WebviewPanelTargetArea.md)

Target area where webview panel will be resided. Shows in the 'WebviewPanelTargetArea.Main' area if undefined.

#### Defined in

[index.d.ts:3516](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3516)

___

### preserveFocus

• `Optional` **preserveFocus**: `boolean`

When `true`, the webview will not take focus.

#### Defined in

[index.d.ts:3526](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3526)

___

### viewColumn

• `Optional` **viewColumn**: `number`

Editor View column to show the panel in. Shows in the current `viewColumn` if undefined.

#### Defined in

[index.d.ts:3521](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3521)
