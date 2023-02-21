[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DecorationRenderOptions

# Interface: DecorationRenderOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DecorationRenderOptions

Represents rendering styles for a [text editor decoration](#TextEditorDecorationType).

## Hierarchy

- [`ThemableDecorationRenderOptions`](cloudide_plugin_.ThemableDecorationRenderOptions.md)

  ↳ **`DecorationRenderOptions`**

## Table of contents

### Properties

- [after](cloudide_plugin_.DecorationRenderOptions.md#after)
- [backgroundColor](cloudide_plugin_.DecorationRenderOptions.md#backgroundcolor)
- [before](cloudide_plugin_.DecorationRenderOptions.md#before)
- [border](cloudide_plugin_.DecorationRenderOptions.md#border)
- [borderColor](cloudide_plugin_.DecorationRenderOptions.md#bordercolor)
- [borderRadius](cloudide_plugin_.DecorationRenderOptions.md#borderradius)
- [borderSpacing](cloudide_plugin_.DecorationRenderOptions.md#borderspacing)
- [borderStyle](cloudide_plugin_.DecorationRenderOptions.md#borderstyle)
- [borderWidth](cloudide_plugin_.DecorationRenderOptions.md#borderwidth)
- [color](cloudide_plugin_.DecorationRenderOptions.md#color)
- [cursor](cloudide_plugin_.DecorationRenderOptions.md#cursor)
- [dark](cloudide_plugin_.DecorationRenderOptions.md#dark)
- [fontStyle](cloudide_plugin_.DecorationRenderOptions.md#fontstyle)
- [fontWeight](cloudide_plugin_.DecorationRenderOptions.md#fontweight)
- [gutterIconPath](cloudide_plugin_.DecorationRenderOptions.md#guttericonpath)
- [gutterIconSize](cloudide_plugin_.DecorationRenderOptions.md#guttericonsize)
- [isWholeLine](cloudide_plugin_.DecorationRenderOptions.md#iswholeline)
- [letterSpacing](cloudide_plugin_.DecorationRenderOptions.md#letterspacing)
- [light](cloudide_plugin_.DecorationRenderOptions.md#light)
- [opacity](cloudide_plugin_.DecorationRenderOptions.md#opacity)
- [outline](cloudide_plugin_.DecorationRenderOptions.md#outline)
- [outlineColor](cloudide_plugin_.DecorationRenderOptions.md#outlinecolor)
- [outlineStyle](cloudide_plugin_.DecorationRenderOptions.md#outlinestyle)
- [outlineWidth](cloudide_plugin_.DecorationRenderOptions.md#outlinewidth)
- [overviewRulerColor](cloudide_plugin_.DecorationRenderOptions.md#overviewrulercolor)
- [overviewRulerLane](cloudide_plugin_.DecorationRenderOptions.md#overviewrulerlane)
- [rangeBehavior](cloudide_plugin_.DecorationRenderOptions.md#rangebehavior)
- [textDecoration](cloudide_plugin_.DecorationRenderOptions.md#textdecoration)

## Properties

### after

• `Optional` **after**: [`ThemableDecorationAttachmentRenderOptions`](cloudide_plugin_.ThemableDecorationAttachmentRenderOptions.md)

Defines the rendering options of the attachment that is inserted after the decorated text

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[after](cloudide_plugin_.ThemableDecorationRenderOptions.md#after)

#### Defined in

[index.d.ts:1069](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1069)

___

### backgroundColor

• `Optional` **backgroundColor**: `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

Background color of the decoration. Use rgba() and define transparent background colors to play well with other decorations.
Alternatively a color from the color registry can be [referenced](#ThemeColor).

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[backgroundColor](cloudide_plugin_.ThemableDecorationRenderOptions.md#backgroundcolor)

#### Defined in

[index.d.ts:949](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L949)

___

### before

• `Optional` **before**: [`ThemableDecorationAttachmentRenderOptions`](cloudide_plugin_.ThemableDecorationAttachmentRenderOptions.md)

Defines the rendering options of the attachment that is inserted before the decorated text

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[before](cloudide_plugin_.ThemableDecorationRenderOptions.md#before)

#### Defined in

[index.d.ts:1064](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1064)

___

### border

• `Optional` **border**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[border](cloudide_plugin_.ThemableDecorationRenderOptions.md#border)

#### Defined in

[index.d.ts:977](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L977)

___

### borderColor

• `Optional` **borderColor**: `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[borderColor](cloudide_plugin_.ThemableDecorationRenderOptions.md#bordercolor)

#### Defined in

[index.d.ts:983](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L983)

___

### borderRadius

• `Optional` **borderRadius**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[borderRadius](cloudide_plugin_.ThemableDecorationRenderOptions.md#borderradius)

#### Defined in

[index.d.ts:989](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L989)

___

### borderSpacing

• `Optional` **borderSpacing**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[borderSpacing](cloudide_plugin_.ThemableDecorationRenderOptions.md#borderspacing)

#### Defined in

[index.d.ts:995](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L995)

___

### borderStyle

• `Optional` **borderStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[borderStyle](cloudide_plugin_.ThemableDecorationRenderOptions.md#borderstyle)

#### Defined in

[index.d.ts:1001](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1001)

___

### borderWidth

• `Optional` **borderWidth**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[borderWidth](cloudide_plugin_.ThemableDecorationRenderOptions.md#borderwidth)

#### Defined in

[index.d.ts:1007](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1007)

___

### color

• `Optional` **color**: `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[color](cloudide_plugin_.ThemableDecorationRenderOptions.md#color)

#### Defined in

[index.d.ts:1032](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1032)

___

### cursor

• `Optional` **cursor**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[cursor](cloudide_plugin_.ThemableDecorationRenderOptions.md#cursor)

#### Defined in

[index.d.ts:1027](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1027)

___

### dark

• `Optional` **dark**: [`ThemableDecorationRenderOptions`](cloudide_plugin_.ThemableDecorationRenderOptions.md)

Overwrite options for dark themes.

#### Defined in

[index.d.ts:1134](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1134)

___

### fontStyle

• `Optional` **fontStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[fontStyle](cloudide_plugin_.ThemableDecorationRenderOptions.md#fontstyle)

#### Defined in

[index.d.ts:1012](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1012)

___

### fontWeight

• `Optional` **fontWeight**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[fontWeight](cloudide_plugin_.ThemableDecorationRenderOptions.md#fontweight)

#### Defined in

[index.d.ts:1017](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1017)

___

### gutterIconPath

• `Optional` **gutterIconPath**: `string` \| [`Uri`](../classes/cloudide_plugin_.Uri.md)

An **absolute path** or an URI to an image to be rendered in the gutter.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[gutterIconPath](cloudide_plugin_.ThemableDecorationRenderOptions.md#guttericonpath)

#### Defined in

[index.d.ts:1047](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1047)

___

### gutterIconSize

• `Optional` **gutterIconSize**: `string`

Specifies the size of the gutter icon.
Available values are 'auto', 'contain', 'cover' and any percentage value.
For further information: https://msdn.microsoft.com/en-us/library/jj127316(v=vs.85).aspx

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[gutterIconSize](cloudide_plugin_.ThemableDecorationRenderOptions.md#guttericonsize)

#### Defined in

[index.d.ts:1054](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1054)

___

### isWholeLine

• `Optional` **isWholeLine**: `boolean`

Should the decoration be rendered also on the whitespace after the line text.
Defaults to `false`.

#### Defined in

[index.d.ts:1113](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1113)

___

### letterSpacing

• `Optional` **letterSpacing**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[letterSpacing](cloudide_plugin_.ThemableDecorationRenderOptions.md#letterspacing)

#### Defined in

[index.d.ts:1042](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1042)

___

### light

• `Optional` **light**: [`ThemableDecorationRenderOptions`](cloudide_plugin_.ThemableDecorationRenderOptions.md)

Overwrite options for light themes.

#### Defined in

[index.d.ts:1129](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1129)

___

### opacity

• `Optional` **opacity**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[opacity](cloudide_plugin_.ThemableDecorationRenderOptions.md#opacity)

#### Defined in

[index.d.ts:1037](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1037)

___

### outline

• `Optional` **outline**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[outline](cloudide_plugin_.ThemableDecorationRenderOptions.md#outline)

#### Defined in

[index.d.ts:954](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L954)

___

### outlineColor

• `Optional` **outlineColor**: `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[outlineColor](cloudide_plugin_.ThemableDecorationRenderOptions.md#outlinecolor)

#### Defined in

[index.d.ts:960](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L960)

___

### outlineStyle

• `Optional` **outlineStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[outlineStyle](cloudide_plugin_.ThemableDecorationRenderOptions.md#outlinestyle)

#### Defined in

[index.d.ts:966](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L966)

___

### outlineWidth

• `Optional` **outlineWidth**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[outlineWidth](cloudide_plugin_.ThemableDecorationRenderOptions.md#outlinewidth)

#### Defined in

[index.d.ts:972](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L972)

___

### overviewRulerColor

• `Optional` **overviewRulerColor**: `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

The color of the decoration in the overview ruler. Use rgba() and define transparent colors to play well with other decorations.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[overviewRulerColor](cloudide_plugin_.ThemableDecorationRenderOptions.md#overviewrulercolor)

#### Defined in

[index.d.ts:1059](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1059)

___

### overviewRulerLane

• `Optional` **overviewRulerLane**: [`OverviewRulerLane`](../enums/cloudide_plugin_.OverviewRulerLane.md)

The position in the overview ruler where the decoration should be rendered.

#### Defined in

[index.d.ts:1124](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1124)

___

### rangeBehavior

• `Optional` **rangeBehavior**: [`DecorationRangeBehavior`](../enums/cloudide_plugin_.DecorationRangeBehavior.md)

Customize the growing behavior of the decoration when edits occur at the edges of the decoration's range.
Defaults to `DecorationRangeBehavior.OpenOpen`.

#### Defined in

[index.d.ts:1119](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1119)

___

### textDecoration

• `Optional` **textDecoration**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](cloudide_plugin_.ThemableDecorationRenderOptions.md).[textDecoration](cloudide_plugin_.ThemableDecorationRenderOptions.md#textdecoration)

#### Defined in

[index.d.ts:1022](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1022)
