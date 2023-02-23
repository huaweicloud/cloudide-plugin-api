[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ThemableDecorationRenderOptions

# Interface: ThemableDecorationRenderOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ThemableDecorationRenderOptions

Represents theme specific rendering styles for a [text editor decoration](#TextEditorDecorationType).

## Hierarchy

- **`ThemableDecorationRenderOptions`**

  ↳ [`DecorationRenderOptions`](cloudide_plugin_.DecorationRenderOptions.md)

## Table of contents

### Properties

- [after](cloudide_plugin_.ThemableDecorationRenderOptions.md#after)
- [backgroundColor](cloudide_plugin_.ThemableDecorationRenderOptions.md#backgroundcolor)
- [before](cloudide_plugin_.ThemableDecorationRenderOptions.md#before)
- [border](cloudide_plugin_.ThemableDecorationRenderOptions.md#border)
- [borderColor](cloudide_plugin_.ThemableDecorationRenderOptions.md#bordercolor)
- [borderRadius](cloudide_plugin_.ThemableDecorationRenderOptions.md#borderradius)
- [borderSpacing](cloudide_plugin_.ThemableDecorationRenderOptions.md#borderspacing)
- [borderStyle](cloudide_plugin_.ThemableDecorationRenderOptions.md#borderstyle)
- [borderWidth](cloudide_plugin_.ThemableDecorationRenderOptions.md#borderwidth)
- [color](cloudide_plugin_.ThemableDecorationRenderOptions.md#color)
- [cursor](cloudide_plugin_.ThemableDecorationRenderOptions.md#cursor)
- [fontStyle](cloudide_plugin_.ThemableDecorationRenderOptions.md#fontstyle)
- [fontWeight](cloudide_plugin_.ThemableDecorationRenderOptions.md#fontweight)
- [gutterIconPath](cloudide_plugin_.ThemableDecorationRenderOptions.md#guttericonpath)
- [gutterIconSize](cloudide_plugin_.ThemableDecorationRenderOptions.md#guttericonsize)
- [letterSpacing](cloudide_plugin_.ThemableDecorationRenderOptions.md#letterspacing)
- [opacity](cloudide_plugin_.ThemableDecorationRenderOptions.md#opacity)
- [outline](cloudide_plugin_.ThemableDecorationRenderOptions.md#outline)
- [outlineColor](cloudide_plugin_.ThemableDecorationRenderOptions.md#outlinecolor)
- [outlineStyle](cloudide_plugin_.ThemableDecorationRenderOptions.md#outlinestyle)
- [outlineWidth](cloudide_plugin_.ThemableDecorationRenderOptions.md#outlinewidth)
- [overviewRulerColor](cloudide_plugin_.ThemableDecorationRenderOptions.md#overviewrulercolor)
- [textDecoration](cloudide_plugin_.ThemableDecorationRenderOptions.md#textdecoration)

## Properties

### after

• `Optional` **after**: [`ThemableDecorationAttachmentRenderOptions`](cloudide_plugin_.ThemableDecorationAttachmentRenderOptions.md)

Defines the rendering options of the attachment that is inserted after the decorated text

#### Defined in

[index.d.ts:1069](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1069)

___

### backgroundColor

• `Optional` **backgroundColor**: `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

Background color of the decoration. Use rgba() and define transparent background colors to play well with other decorations.
Alternatively a color from the color registry can be [referenced](#ThemeColor).

#### Defined in

[index.d.ts:949](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L949)

___

### before

• `Optional` **before**: [`ThemableDecorationAttachmentRenderOptions`](cloudide_plugin_.ThemableDecorationAttachmentRenderOptions.md)

Defines the rendering options of the attachment that is inserted before the decorated text

#### Defined in

[index.d.ts:1064](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1064)

___

### border

• `Optional` **border**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:977](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L977)

___

### borderColor

• `Optional` **borderColor**: `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Defined in

[index.d.ts:983](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L983)

___

### borderRadius

• `Optional` **borderRadius**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Defined in

[index.d.ts:989](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L989)

___

### borderSpacing

• `Optional` **borderSpacing**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Defined in

[index.d.ts:995](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L995)

___

### borderStyle

• `Optional` **borderStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Defined in

[index.d.ts:1001](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1001)

___

### borderWidth

• `Optional` **borderWidth**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Defined in

[index.d.ts:1007](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1007)

___

### color

• `Optional` **color**: `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:1032](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1032)

___

### cursor

• `Optional` **cursor**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:1027](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1027)

___

### fontStyle

• `Optional` **fontStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:1012](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1012)

___

### fontWeight

• `Optional` **fontWeight**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:1017](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1017)

___

### gutterIconPath

• `Optional` **gutterIconPath**: `string` \| [`Uri`](../classes/cloudide_plugin_.Uri.md)

An **absolute path** or an URI to an image to be rendered in the gutter.

#### Defined in

[index.d.ts:1047](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1047)

___

### gutterIconSize

• `Optional` **gutterIconSize**: `string`

Specifies the size of the gutter icon.
Available values are 'auto', 'contain', 'cover' and any percentage value.
For further information: https://msdn.microsoft.com/en-us/library/jj127316(v=vs.85).aspx

#### Defined in

[index.d.ts:1054](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1054)

___

### letterSpacing

• `Optional` **letterSpacing**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:1042](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1042)

___

### opacity

• `Optional` **opacity**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:1037](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1037)

___

### outline

• `Optional` **outline**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:954](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L954)

___

### outlineColor

• `Optional` **outlineColor**: `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Defined in

[index.d.ts:960](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L960)

___

### outlineStyle

• `Optional` **outlineStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Defined in

[index.d.ts:966](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L966)

___

### outlineWidth

• `Optional` **outlineWidth**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Defined in

[index.d.ts:972](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L972)

___

### overviewRulerColor

• `Optional` **overviewRulerColor**: `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

The color of the decoration in the overview ruler. Use rgba() and define transparent colors to play well with other decorations.

#### Defined in

[index.d.ts:1059](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1059)

___

### textDecoration

• `Optional` **textDecoration**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:1022](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1022)
